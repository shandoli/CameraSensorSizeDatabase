
Camera Sensor Size Database
===========================

An open camera sensor size database.

------------
Introduction
------------

This repository contains a list of camera model and their corresponding camera sensor size.

Linking image entry to image EXIF data allow to compute approximate focal length (in pixels)

focal_pix = (max( w, h ) * focal_mm) / ccdw_mm

  - focal_pix: the focal length in pixels,
  - focal_mm: the EXIF focal length (mm),
  - w,h  the image of width and height (pixels),
  - ccdw_mm: the known sensor width size (mm).

-----------
Description
-----------

There are two flavors of the database.

The sensor_database.csv has the format

    CameraMaker,CameraModel,SensorWidth(mm)

The sensor_database_detailed.csv

    CameraMaker,CameraModel,SensorDescription,SensorWidth(mm),SensorHeight(mm),SensorWidth(pixels),SensorHeight(pixels)


Contributions to the database are welcome (please use the pull request mechanism)


-------
License
-------

The database is available under the MIT license, see the [LICENSE](https://github.com/openMVG/cameraSensorSizeDatabase/raw/master/LICENSE) text file.
