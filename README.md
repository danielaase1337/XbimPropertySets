# Xbim.PropertySets

Subproject of https://github.com/xBimTeam/

## What is it?

The xBIM Tookit (eXtensible Building Information Modelling) is an open-source, software development BIM toolkit that 
supports the BuildingSmart Data Model (aka the [Industry Foundation Classes IFC](http://en.wikipedia.org/wiki/Industry_Foundation_Classes)).

xBIM allows developers to read, create and view [Building Information (BIM)](http://en.wikipedia.org/wiki/Building_information_modeling) Models in the IFC format. 
There is full support for geometric, topological operations and visualisation. In addition xBIM supports 
bi-directional translation between IFC and COBie formats

## Getting Started

This package is independent so you can use it standalone. It implements buildingSMART data model for description of property and quantity sets. It also contains these definitions
taken from buildingSMART as a resources so you can just take it and instantiate all predefined property sets for IFC2x3 or IFC4. It is as simple as this:

    var defs = new Definitions<PropertySetDef>(Version.IFC4);
    defs.LoadAllDefault();
    var prop = defs["Pset_ActionRequest"]["RequestSourceName"] as PropertyDef;


Xbim is a software library, and is currently deployed with a number of sample applications to demonstrate its capabilities

* XbimXplorer - a Windows WPF sample application that can open and render 3D IFC models (and native XBIM models ) as well as displaying semantic data.
* Xbim.SceneJSWebViewer - a MVC web application that can open and render 3D IFC models (previously converted to XBIM) using a WebGL compatible browser. 
* XbimConvert - a sample console application to generate native XBIM model and geometry files from an IFC file.
* Xbim.COBie.Client - A sample windows application demonstrating how a COBie spreadsheet can be generated from an IFC model.
* CodeExamples - a sample console application demonstrating how to undertake a number of BIM processes using XBIM

Please note: all the samples in this solution are examples of how to use the Xbim library, and not intended to be used in a 
production environment without further development.

## Licence

The XBIM library is made available under the CDDL Open Source licence.  See the licences folder for a full text.

All licences should support the commercial usage of the XBIM system within a 'Larger Work', as long as you honour 
the licence agreements.

## Third Party Licences

The core XBIM library makes use of the following 3rd party software packages, under their associated licences:

* 'OpenCASCADE' Geometry Engine : http://www.opencascade.org/ - OPEN CASCADE Public License 
* 'Gardens Point Parser Generator' http://gppg.codeplex.com/ - New BSD Licence
* Elements of '3D Tools' WPF library http://3dtools.codeplex.com/ - MS Permissive Licence
* Log4net : http://logging.apache.org/log4net/ - Apache 2.0 Licence
* NPOI : http://npoi.codeplex.com - Apache 2.0 Licence
* NewtonSoft JSON : http://json.codeplex.com/ - MIT Licence

Additionally the Samples also make use of the following libraries

* SceneJS: https://github.com/xeolabs/scenejs - joint MIT and GPL Licence
* SignalR : https://github.com/SignalR/SignalR - Apache 2.0 Licence

All licences are included in full under the Licences\3rd Party solution folder. 


