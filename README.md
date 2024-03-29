# Microsoft Project Acoustics
This repository provides a communication channel for customers using [Project Acoustics](https://aka.ms/acoustics).

* [Issue Tracking](https://github.com/microsoft/ProjectAcoustics/issues)
    * [Notices](https://github.com/microsoft/ProjectAcoustics/labels/notice)
    * [Known issues](https://github.com/microsoft/ProjectAcoustics/labels/known%20issue)
    * [Questions](https://github.com/microsoft/ProjectAcoustics/labels/question)
    
## RELEASE UPDATE (November 17, 2022):

We're happy to announce that a new version of Project Acoustics is available! It includes many bug fixes and new features. The documentation has been updated at http://aka.ms/acoustics with information about new features and beta features. Here's a few highlights:

## Version 2022.1 - November 2022
* Full Unreal Marketplace and Download Center release
* BREAKING CHANGES - Triton encoder updated to 4.0.0 from 3.02.01, removed Distance Warp design parameter
* General
    * Migrate to VS2022
    * Year-based version scheme
* HRTF PROCESSING
    * Shared results from FLEX listening test in Journal of the Acoustic Engineering Society
* TRITON
    * New Voxel-free interpolator. Voxels only kept around for debug visuals. New interpolation API provides various modes to handle queries near geometry appropriately
    * Visualizer updated to support parameter field interpolation logic
    * Load multiple ACE files simultaneously at runtime
    * Moved API inputs and mesh parsing to double precision to support large worlds
* UNREAL
    * Spatial reverb support in Unreal Audio plugin
    * New FLEX-based spatializer plugin
    * Expose Project Acoustics parameters to MetaSounds
    * UX for setting new interpolation modes
    * Support for UE5.1
    * Support for Android
    * Fix for portalling support with UE built-in panning
    * Fix for Python installation (support latest PythonNet)
    * Fix for custom IRs saving properly
* WWISE
    * Spatial reverb plugin
    * Support Wwise 2022.1

## Downloads

* [Unity plug-in Download](https://www.microsoft.com/en-us/download/details.aspx?id=57346)
* [Unreal+Wwise plug-in Download](https://www.microsoft.com/en-us/download/details.aspx?id=58090)
* [Unreal Engine 5/5.1 plug-in on the Marketplace](https://www.unrealengine.com/marketplace/en-US/product/06cfe91228c04848a0f6d6f7fb7b40f0)

## Resources

* [Microsoft Project Acoustics UE5 Marketplace Plugin | Inside Unreal](https://youtu.be/3uocCX0AMIg)
* [Mixed Reality Dev Days 2020 Session on Project Acoustics with HoloLens 2](https://channel9.msdn.com/Shows/Mixed-Reality/Using-Project-Acoustics-with-HoloLens-2)
* [The GDC 2019 Session on Project Acoustics](https://www.youtube.com/watch?v=uY4G-GUAQIE&feature=youtu.be&list=PLRs2lXTYCDQ3q9WF-4aO2SgCCCL6rSmA6)
* [Technical overview](https://docs.microsoft.com/en-us/gaming/acoustics/what-is-acoustics)
* [Making Waves with Triton](https://youtu.be/pIzwo-MxCC8)

* * *

# Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

# Legal Notices

Microsoft and any contributors grant you a license to the Microsoft documentation and other content
in this repository under the [Creative Commons Attribution 4.0 International Public License](https://creativecommons.org/licenses/by/4.0/legalcode),
see the [LICENSE](LICENSE) file, and grant you a license to any code in the repository under the [MIT License](https://opensource.org/licenses/MIT), see the
[LICENSE-CODE](LICENSE-CODE) file.

Microsoft, Windows, Microsoft Azure and/or other Microsoft products and services referenced in the documentation
may be either trademarks or registered trademarks of Microsoft in the United States and/or other countries.
The licenses for this project do not grant you rights to use any Microsoft names, logos, or trademarks.
Microsoft's general trademark guidelines can be found at http://go.microsoft.com/fwlink/?LinkID=254653.

Privacy information can be found at https://privacy.microsoft.com/en-us/

Microsoft and any contributors reserve all other rights, whether under their respective copyrights, patents,
or trademarks, whether by implication, estoppel or otherwise.
