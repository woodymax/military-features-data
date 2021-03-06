# military-features-data

The ArcGIS Defense and Intelligence Military Features Data repository is a set of data and test applications for use in ArcGIS Desktop and ArcGIS Runtime. This data is used to create features for planning, operations and intelligence domains based on military symbology specifications such as MIL-STD-2525C and APP-6(B).

![Image of Military Features Data](ScreenShot.png)

## Features

* This is the source data for the ArcGIS Defense and Intelligence military feature templates. This data is used to create features and derived data products using military symbology. 
* Provides data files that let you create command and control (C2) operational features based on military symbology specifications MIL-STD-2525C/D and APP-6(B) in ArcGIS Desktop
* Provides project/layer packages that include the database schema and sample data for military features
* Provides symbology style files for displaying and creating military symbology in ArcGIS Desktop
* Provides additional derived data products for use in ArcGIS Runtime
* See each version of the standard for more information:
    * [US MIL-STD-2525D "Delta" - mil2525d](./data/mil2525d)
    * [US MIL-STD-2525C "Charlie" - mil2525c](./data/mil2525c)
    * [NATO APP-6(B) - app6b](./data/app6b)
    * Important Note: MIL-STD-2525D is the current and actively maintained version. Other older standard versions are provided for legacy purposes.

## Sections

* [Requirements](#requirements)
* [Instructions](#instructions)
* [Resources](#resources)
* [Issues](#issues)
* [Contributing](#contributing)
* [Licensing](#licensing)

## Requirements

* ArcGIS Desktop 10.1+ 
    * If using the Style and Layer Files
* ArcGIS Runtime 10.2 (or later)
    * If using the Symbol Dictionary Files
* ArcGIS Pro 1.2+ or ArcGIS Runtime Quartz
    * If using the Stylx Files or Dictionary Renderers

## Instructions

### General Help

[New to Github? Get started here.](http://htmlpreview.github.com/?https://github.com/Esri/esri.github.com/blob/master/help/esri-getting-to-know-github.html)

### Using the Source Data

* Download the repository
* Determine the version of the military symbology standard you are using:
    * [US MIL-STD-2525D "Delta" - mil2525d](./data/mil2525d)
    * [US MIL-STD-2525C "Charlie" - mil2525c](./data/mil2525c)
    * [NATO APP-6(B) - app6b](./data/app6b)
* If using the source data with ArcGIS Runtime or ArcGIS Professional...
    * If you are using MIL-STD-2525D "Delta" with ArcGIS Pro there is no additional configuration required - this is included with the product
        * You may simply start using one of the included packages, templates, or other test data at
            * [data/mil2525d/overlay_templates](./data/mil2525d/overlay_templates)
            * [data/mil2525d/test_data](./data/mil2525d/test_data)
    * If you are using an older version of the military standard, you will likely need to update/configure the local ArcGIS files with the versions from this repository.
    * Navigate to the appropriate folder (based on the standard/version desired) in this repository:
    * If you would like to use a Dictionary Renderer, navigate to
        * [data\mil2525c\stylxfiles](./data/mil2525c/dictionaryrenderer)
        * [data\app6b\stylxfiles](./data/app6b/dictionaryrenderer)
    * If you would like to use just the .stylx file, navigate to
        * [data\mil2525c\stylxfiles](./data/mil2525c/stylxfiles)
        * [data\app6b\stylxfiles](./data/app6b/stylxfiles)
    * Update/copy the files from each folder into your local resource folder. E.g.
        * ArcGIS Professional: `Pro\Resources\Dictionaries\{standard}`
        * ArcGIS Runtime: `arcgisruntimeX.X.X\resources`
        * Overwrite if necessary (but you may want to create a backup of these files before this step)
* If using the source data with ArcGIS Desktop(ArcMap)...
    * Update the local ArcGIS Military Style Files to the latest versions from the repository.
        * Navigate to the folders
            *  [military-features-data\data\mil2525d\stylefiles](./data/mil2525d/stylefiles)
            *  [military-features-data\data\mil2525c\stylefiles](./data/mil2525c/stylefiles)
            *  [military-features-data\data\app6b\stylefiles](./data/app6b/stylefiles)
        * Update/copy all of the .style files from each folder into your ArcGIS Desktop Style folder (overwrite if necessary - it is highly recommended that you create a backup of these files before this step)
        * For example, copy the style files from above location into this Desktop Folder: `{ArcGIS Install Location}\ArcGIS\Desktop10.X\Styles`
    * Create symbology using the ArcGIS Style Manager or open the provided layer packages to create military features

### Running the ArcGIS Runtime Test Applications

* There are several sample/test applications provided for the standalone test/verification/validation of this data.
* For more information, see the instructions in the [test](./test) folder.

## Resources

* The [Official Military Standard Documents](http://quicksearch.dla.mil/qsDocDetails.aspx?ident_number=114934)
* [ArcGIS Solutions](http://solutions.arcgis.com/)
* [ArcGIS Pro Dictionary Renderer Help Page](https://pro.arcgis.com/en/pro-app/help/mapping/symbols-and-styles/dictionary-renderer.htm) 
* [ArcGIS Military Features Help Documentation](http://resources.arcgis.com/en/help/main/10.1/index.html#//000n0000000p000000)
* Military Features Blog Posts 
    * [Quick Introduction](http://blogs.esri.com/esri/arcgis/2011/02/18/a-quick-introduction-to-text-modifiers-for-unit-equipment-and-installation-features/)
    * [Creating New Symbols](http://blogs.esri.com/esri/arcgis/2011/02/04/representing-c2-tactical-symbols-in-arcgis-as-uei-features/)
    * [Symbol ID Codes](http://blogs.esri.com/esri/arcgis/2010/05/19/military-features-and-symbol-id-codes/)
    * [Direction Indicator](http://blogs.esri.com/esri/arcgis/2011/04/01/creating-a-direction-of-movement-graphic-modifier/)
* Learned more about Esri's [Solutions Templates](http://solutions.arcgis.com/)
* Learn more about Esri's [ArcGIS for Defense maps and apps](http://resources.arcgis.com/en/communities/defense-and-intelligence/).

## Issues

* Find a bug or want to request a new feature?  Please let us know by submitting an issue.

## Contributing

Esri welcomes contributions from anyone and everyone. Please see our [guidelines for contributing](https://github.com/esri/contributing).

## Licensing

Copyright 2013-2015 Esri

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

A copy of the license is available in the repository's
[license.txt](license.txt) file.

[](Esri Tags: ArcGIS Defense Intelligence Military Features 2525 APP6 2525C 2525D APP6B ArcGISSolutions)
[](Esri Language: Java)
