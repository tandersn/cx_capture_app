# cx_capture_app:  EXPERIMENTAL!! ALPHA PHASE!!
A linux GUI capture application for connexant cx2338[0/1/2/3] and cx25800 based cards

# Information:

  You will need to install GNU Radio Companion for this to work, and any depndencies it needs.
  You will need the cxadc driver that supports `center_offset` value, which as of this writing is only my version.




Still very experimental. Not sure if this is the best way to develop a capture app for cxadc, it's just what i could get done quickly. I also have tested A/B capturing with this and straight `cat /dev/cxadc0`.  It is not impossible for gnuradio to drop samples.


# Limitations:
  16 bit mode is not support
  auto adjustment of level not support (like how cxlvlcavdd does for CAV discs). As such, probably not best solution for CAV discs.



