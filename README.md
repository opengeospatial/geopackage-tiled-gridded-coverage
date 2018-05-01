# OGC GeoPackage Extension for Tiled Gridded Coverage Data

OGC document reference: 17-066

This GitHub repository contains the content for the OGC "GeoPackage Extension for Tiled Gridded Coverage Data” extension. The extension (previously titled Elevation Extension)" defines how to encode and store tiled regular gridded data, such as a digital elevation model, in a GeoPackage. In the ISO 19123 Schema for Coverage Geometry standard and in the OGC Coverage Implementation Schema, this type of regular gridded data is classed as `grid-regular` footnote:[Grid-regular in OGC Coverage Implementation Schema (CIS). More specifically, for a continuous grid-regular coverage, see CV_ContinuousQuadrilateralGridCoverage in ISO 19123 and OGC Topic Volume 6.]. The tiles contain values, such as elevation, temperature or pressure, and may be stored as 16-bit PNG files or 32-bit TIFF files. The extension defines two ancillary data tables: one for regular gridded coverages and one for tiles. When using the PNG encoding, a scale and offset may be applied. The extension also allows for a TIFF encoding but constrains many of the TIFF options that are available to simplify development.

The published version of this document is at http://docs.opengeospatial.org/is/17-066r1/17-066r1.html.

The entry point is [./standard/standard_document.adoc](./standard/standard_document.adoc)

For contributors, the repo is organized as follows:

* standard - the main standard document content
  - organized in multiple sections and directories
  - this is the only part needed to create a standard
* code - sample code to accompany the standard, if desired
* abstract_tests - the Abstract Test Suite comprising one test for every requirement, optional
* UML - UML diagrams, if applicable
