Projects
================

[Course Home](../README.md) | [General Info](general-information.md) |
[Syllabus](syllabus.md) | [Intro Modules](introductory-modules.md)

# Team Projects

There are several potential projects that can be undertaken for this
class.

1.  [Multi-scale estimation of crop LAI](#project-1)
2.  [Multi-scale estimation of crop yield](#project-2)
3.  [Using cloud-based EO processing platforms to create multi-source
    image time series](#project-3)
4.  [Mapping land cover using crowdsourcing and machine
    learning](#project-4)
5.  [Drone mapping Hadwen Arboretum](#project-5)

More detail on each follows:

## Project 1

### Maize Leaf Area Index

We have been collecting data over the course of the summer in a
maize/corn field at Whittier Farms, in Sutton, MA. Data include:

  - Micro-meteorology and crop growth data collected by three Arable
    Mark sensors over two seasons
  - Field measurements of leaf area index collected underneath each Mark
    (two seasons)
  - 10 cm multi-spectral imagery collected by a Sequioa+ camera mounted
    on an Ebee Plus UAS on several dates (two seasons)

In addition to these, we can also acquire near-daily PlanetScope 3-4
RGBNIR imagery over the same fields for the same years.

One major goal of this project is to develop estimates of maize leaf
area index (LAI) from these multiple sources and understand how these
estimates change with scale and extent. To do this, we will:

  - Derive measurements of LAI first from the field measurements;
  - Use these measurements to estimate LAI values from the Marks’
    spectrometer data, and co-located UAS and PlanetScope image pixels;
  - Apply the UAS and PlanetScope LAI-image relationships to map LAI
    across the fields at varying resolution;
  - Quantify the discrepancies between the various LAI estimation
    approaches.

Along the way, we will make additional use of our Mark data to convert
PlanetScope imagery to surface reflectance, perhaps with topographic
normalization thrown in for good measure.

## Project 2

### Maize yield

This project is closely related to project 1, in that it will rely in
part on the LAI estimates. For this project, we want to:

  - Use the Mark micro-meteorology estimates to run a mechanistic crop
    simulator to predict maize yields.
  - Use the mechanistic model outputs (including simulated LAI) and a
    subset of simplified inputs to develop an empirical model of
    yields.  
  - Using these relationships together with remotely-sensed predictors
    (primarily LAI), we will map predicted yields in \~16-25
    m<sup>2</sup> blocks through the fields.

## Project 3

### EO Platforms and High Resolution Image Time Series

One ongoing research need for estimating agricultural productivity is to
have a set of imagery that is:

1.  High resolution (\<=30 m)
2.  High frequency (\<1 month return)
3.  Covers a number of years.

New satellite fleets such as those of Planet enable 1 and 2, but not 3,
which is necessary for studying changes in productivity over time.

There are new approaches that allow the fusion of MODIS and Landsat
data, where MODIS provides the temporal resolution and Landsat the
spatial. Both sets of imagery are available in new cloud-based
processing engines such as Google Earth Engine.

In this project, we aim to develop such a dataset for Zambia, using a
new approach such as
[STAIR](https://www.sciencedirect.com/science/article/pii/S0034425718301998)
(Luo et al, 2018).

This could be done in EarthEngine or EarthAI notebooks.

## Project 4

### Active Learning

We are developing a new land cover mapping platform that runs on Amazon
Web Services virtual machines. The platform is based on active learning,
where a machine learning algorithm iteratively tasks human mappers to
collect training data in areas of lingering classification uncertainty.
The mappers create this training data by digitizing crop fields they
identify in high resolution Planet imagery.

There are three possible projects related to this:

1.  Deploy the active learning framework to a new geography outside of
    the current target region (Ghana).
2.  Apply it to new land cover type.
3.  Use the training datasets and imagery collected for Ghana to
    investigate the impact that training data error has on
    classification accuracy.

### Deep learning

Apply a deep learning model to develop a classification map. One
approach might be to try adapt this approach
[here](https://github.com/microsoft/landcover) to get it running on a
local or AWS server, and then point it at a new geography (e.g. Ghana).

## Project 5

### Map [Hadwen Arboretum](https://en.wikipedia.org/wiki/Hadwen_Arboretum)

This is UAS-based project, and requires action from the beginning of the
semester. Project outline:

  - Identify correct UAS multicopter for the job, purchase
  - Get FAA clearances to fly
  - Conduct test flights
  - Plan and conduct arboretum flights (late Spring)
  - Create orthomosaic, DTM, DEM, etc.

![](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ef/HadwenArboretum.jpg/1280px-HadwenArboretum.jpg)

## References

Luo, Y., Guan, K., Peng, J., 2018. STAIR: A generic and fully-automated
method to fuse multiple sources of optical satellite data to generate a
high-resolution, daily and cloud-/gap-free surface reflectance product.
Remote Sensing of Environment 214, 87–99.
<https://doi.org/10.1016/j.rse.2018.04.042>

[Course Home](../README.md) | [General Info](general-information.md) |
[Syllabus](syllabus.md) | [Intro Modules](introductory-modules.md)
