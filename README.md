# brother_ql-mk

Python package for the raster language protocol of the Brother QL and PL series label printers


## FORK NOTICE

### brother_ql-inventree

This is a fork of https://github.com/pklaus/brother_ql by [Philipp Klaus](https://github.com/pklaus) to enable faster updates.
Check out https://github.com/inventree/inventree to see what I forked it for.

### brother_ql-mk

This is a further fork of brother_ql-inventree to modify some PL series label printer related functionalities.

## Verified models
### Verified devices

List them with command `brother_ql info models` or see the models.py file.

### Verified labels

List them with command `brother_ql info labels` or see the labels.py file.

### Backends

There are multiple backends for connecting to the printer available (✔: supported, ✘: not supported):

Backend | Kind | Linux | Mac OS | Windows
-------|-------|---------|---------|--------
network (1) | TCP | ✔ | ✔ | ✔
linux\_kernel | USB | ✔ (2) | ✘ | ✘
pyusb (3) | USB | ✔ (3.1) | ✔ (3.2) | ✔ (3.3)

Warning: when using one of the USB backends make sure the Editor Lite feature is turned off (if your model supports it), otherwise the USB Printer interface won't be detected.

## Significant Changes:

### brother_ql-mk

(versions re-begin with v0.9)

### brother_ql-inventree

v1.2:
- Remove support for Python 2 https://github.com/matmair/brother_ql-inventree/pull/43 / https://github.com/matmair/brother_ql-inventree/pull/45
- Added support for PT-E550W https://github.com/matmair/brother_ql-inventree/pull/44
- Added label support for 12+17 https://github.com/matmair/brother_ql-inventree/pull/42
v1.1:
- Support for Pillow 10.x https://github.com/matmair/brother_ql-inventree/pull/37
v1.0:
- Renamed the package to `brother_ql-inventree` and added a release action https://github.com/matmair/brother_ql-inventree/pull/16
- Added printer support for QL-600 https://github.com/matmair/brother_ql-inventree/pull/17 , PT-P950NW https://github.com/matmair/brother_ql-inventree/pull/6 , QL-1100, L-1100NWB, QL-1115NWB https://github.com/matmair/brother_ql-inventree/pull/18
- Added label support for DK-1234 https://github.com/matmair/brother_ql-inventree/pull/22 , 54x29  https://github.com/matmair/brother_ql-inventree/pull/19 , DK22246 https://github.com/matmair/brother_ql-inventree/pull/20, ...

Read the full old Readme [here](https://github.com/matmair/brother_ql-inventree/blob/cleanup/OLD_README.md).
