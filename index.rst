#######################################################
OME Data Model and File Formats |version| Documentation
#######################################################

This documentation covers the OME Data Model, OME-XML and OME-TIFF. 

The OME Model is a specification for storing data on biological imaging.
The model includes image parameters, such as XYZ dimensions and pixels type,
as well as extensive metadata on, for example, image acquisition, annotation,
and regions of interest (ROIs). This common specification is essential
for the exchange of image data between different software packages. OME-XML is
a file format used to store data according to the OME Model, serving as a
convenient file format for data migration from one site or user to another.
OME-TIFF is a multi-plane tiff file that contains OME metadata in the header,
in the form of OME-XML. This allows the pixels to be read with any
TIFF-compatible program, and the metadata to be extracted with any OME-aware
application. Our `paper describing the design and implementation of the OME-XML file 
<https://genomebiology.biomedcentral.com/articles/10.1186/gb-2005-6-5-r47>`_
appeared in Genome Biology.

The OME consortium currently provides three major tools capable of working
with OME-XML and OME-TIFF:

-  The :bf:`Bio-Formats <>` library is a full-featured library with many
   features related to OME-XML, including conversion of third party file
   format metadata into OME-XML structures. It can write image data to the
   OME-TIFF format.

-  :ome-files:`OME Files C++ <>` is a reference implementation of the OME
   data model and OME-TIFF for C++ developers wishing to support these in 
   their own software. It can read and write OME-TIFF data.

-  The :omero:`OMERO server <>` works directly with OME-XML. It can
   import data from OME-XML and OME-TIFF, as well as export to OME-TIFF.


If you have used OME-XML, OME-TIFF, Bio-Formats or OMERO in your work please
use the :citing:`correct citations <>` to acknowledge us.

We have received support from several companies who use our file formats, for
details see our list of :partners:`Partners <>`.

.. note:: The versioning for this documentation reflects updates to any of the
    components it covers and is therefore incremented more frequently than the
    Schema version, which only covers the Data Model and for which a version
    history is provided below.

********
OME-TIFF
********

.. toctree::
    :maxdepth: 1
    :titlesonly:

    ome-tiff/index
    ome-tiff/file-structure
    ome-tiff/specification
    ome-tiff/code
    ome-tiff/data


*******
OME-XML
*******

.. toctree::
    :maxdepth: 1
    :titlesonly:

    ome-xml/index
    ome-tiff/tools
    ome-xml/java-library

*************
OMERO Pyramid
*************

.. toctree::
    :maxdepth: 1
    :titlesonly:

    omero-pyramid/index

*******************
File specifications
*******************

.. toctree::
    :maxdepth: 1
    :titlesonly:

    specifications/index
    specifications/compliant-hcs 
    specifications/minimum


******************************
Developer tools and guidelines
******************************

.. toctree::
    :maxdepth: 1
    :titlesonly:

    developers/index
    developers/using-ome-xml
    developers/compression
    developers/sample-files
    developers/id-and-lsid
    developers/ome-units

************************
The Data Model in detail
************************

Generated documentation for the :schema_doc:`current version of the entire
Schema <ome.html>` is also available.

.. toctree::
    :maxdepth: 1
    :titlesonly:

    developers/model-overview
    developers/filter-and-filterset
    developers/screen-plate-well
    developers/structured-annotations
    developers/roi
    developers/6d-7d-and-8d-storage
    developers/legacy/index


******************
Data Model history
******************

.. toctree::
    :maxdepth: 1
    :titlesonly:

    schemas/index
    schemas/transformations
    schemas/june-2016-2
    schemas/june-2016
    schemas/january-2015
    schemas/june-2013
    schemas/june-2012
    schemas/june-2011
    schemas/june-2010
    schemas/april-2010
    schemas/september-2009
    schemas/september-2008
    schemas/february-2008
    schemas/june-2007-2
    schemas/june-2007

.. toctree::
    :hidden:

    schemas/september-2007
