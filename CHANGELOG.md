## 2022.1 - November 2022
* Full Unreal Marketplace and Download Center release
* BREAKING CHANGES - Triton encoder updated to 3.11.01 from 3.02.01, removed Distance Warp design parameter
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

## 3.0 Patch - June 2022
* Few critical bug fixes for the 3.0 release
* UNREAL
    * Added clamp to prevent reverb from clipping in Marketplace plugin
    * Changed pre-bake default save directory to be in the Project/Plugins directory 
    * Fix for ACE file drag and drop
    * Fix for AcousticsSpace transforms
* TRITON
    * Temporary fix for Android crash in Triton runtime
## 3.0 - May 2022
* Full Marketplace and Download Center release
* HRTF PROCESSING
    * FLEX near-field MVP
* UNITY
    * Fixed Newtonsoft conflict
* UNREAL
    * Added UE5 sample scene
    * Add support for AcousticsSpace translation/rotation
    * New local bake workflow through bake tools from Download Center
    * Triton bake logs from Azure are autodownloaded to Project/Saved directory
    * UE5 native plugin is compilable for the UE Marketplace
## 3.0 Early Access - March 2022
* BREAKING CHANGES - lots of moving pieces in this update, see individual sections below for details of all breaking changes.
* HRTF PROCESSING
    * Latest version of FLEX is available - significant performance boost for same HRTF quality
    * This is the new 'Windows Sonic for Headphones' implementation being ported to Xbox Series hardware
* TRITON
    * BREAKING CHANGE: ALL ACE FILES, JOB PARAMETER JSONs, WILL NEED TO BE REGENERATED
    * Compression Update - ZFP Adaptive
    * New Acoustic Parameters - Direction + Spread Reverb encoding
    * Prebake scalability improvements
    * Job parameter API simplification
    * Bake time optimizations
    * Run-time is now thread-safe (caution: do not use more than 3 concurrent threads -- performance will suffer)
* UNITY
    * Android ARM64 support
* UNREAL ENGINE
    * UE5 native audio engine support via Source Data Override plugin, co-developed with Epic
    * UE5 + Wwise support
    * UE4.27 + Wwise support
    * Moved all Triton queries off game thread to background thread for all UE versions
* WWISE
    * Wwise 2021 Support
    * Mixer plugin has been removed in favor of object processor for versions 2021+
    * Binauralizer Object Processor plugin using latest FLEX engine
    * Automated setup of convolution busses for use with Triton
    * Stub for Spatial Reverb plugin is available in source. Will be fully hooked up once research is complete
* MISC
    * Azure Batch binaries updated to latest
    * /stage option removed from buildandpackage.py -- no longer needed before calling any /package options
    * /Research build config renamed /Checked
    * Android NDK upgraded to R21E
    * GDK support
    * Linux builds upgraded to ubuntu 20.04
    * FBX SDK upgraded to version 2020
    * ThirdPartyNotices.txt moved to repo root for easy reference
## 2.1 - February 2021
* Beta version of FLEX engine type added to HrtfEngine and exposed through Unity plugin.
## 2.0 - February 2021
* BREAKING CHANGE. Replaced managed Triton implementations with native versions. CreateTaskImage deprecated. Pre-2.0 ACE files will still work with 2.0 runtime. Pre-2.0 pre-bake files will **not** work with 2.0 Triton bake tools. Pre-2.0 bake scheduling tools will **not** work with post-2.0 bake tools, and vice versa will also not work.
* Unreal - Additional probe spacing volume types (horizontal probe spacing, material override)
* FBX Importer only: Flood-fill volumes
## 1.2  - March 2020
* First round of Triton bake optimizations from MSR
* Windows Docker support
* Alpha support for doors and pinned probes in Unreal
* Added plugin for VST
* Unity + Wwise support
## 1.1 - July 2019
* MacOS Unity support
* Optimized Unity pre-bake
* Improved HrtfDsp performance
* ACE file streaming
## 1.0 - March 2019
* GDC 2019 release
* Unreal + Wwise support
## 0.5 - August 2018
* Designer Preview. AVAR.
* Unity support

