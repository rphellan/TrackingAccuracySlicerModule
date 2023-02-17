cmake_minimum_required(VERSION 3.16.3...3.19.7 FATAL_ERROR)

project(TrackingErrorIsosurface)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://www.slicer.org/wiki/Documentation/Nightly/Extensions/TrackingErrorIsosurface")
set(EXTENSION_CATEGORY "Tracking Accuracy")
set(EXTENSION_CONTRIBUTORS "Pavel-Dumitru Cernelev (Perklab)")
set(EXTENSION_DESCRIPTION "This extension will generate iso-surfaces representing the accuracy of the tracking methods.")
set(EXTENSION_ICONURL "https://www.example.com/Slicer/Extensions/TrackingErrorIsosurface.png")
set(EXTENSION_SCREENSHOTURLS "https://www.example.com/Slicer/Extensions/TrackingErrorIsosurface/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(DataCollection)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
