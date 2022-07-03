# cx_capture_app:  EXPERIMENTAL!! ALPHA PHASE!!
A linux GUI capture application for connexant cx2338[0/1/2/3] and cx25800 based cards.

# Information:

  You will need to install GNU Radio Companion for this to work, and any depndencies it needs. The installation instructions for your distro can be found by searching google.
  You will need the cxadc driver that supports `center_offset` value, which as of this writing is only my version: https://github.com/tandersn/cxadc-linux3
  Use the `center_offset` value to correct for non-centered singals.
  The scale of the graph is +127 to -127, the `100` notations on the amplitude axis do not represent `100%`.
  You'll need to have granted yourself read access to /dev/cxadc0 and read/write access to the cxadc sysfs parameters (be in `admin` group).


# WARNING!!! 
  Still very experimental. Not sure if this is the best way to develop a capture app for cxadc, it's just what i could get done quickly. I also haven't tested A/B capturing with this and straight `cat /dev/cxadc0`. 

# Limitations:
  16 bit mode is not support.
  Auto adjustment of level not support (like how cxlvlcavdd does for CAV discs). As such, probably not best solution for CAV discs.
  Can't change vmux from within the program (this would require further updates to cxadc driver to allow real time vmux change). Also, vmux changes won't be recognized while the program is running.



 



