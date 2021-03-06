Lag-time and pick correction
============================

The following is a work-in-progress tutorial for lag-calc functionality.

An important note
-----------------
Picks generated by lag-calc are relative to the start of the template waveform,
for example, if you generated your templates with a pre_pick of 0.2, you
should expect picks to occur 0.2 seconds before the actual phase arrival.
The result of this is that origin-times will be shifted by the same amount.

If you have applied different pre_picks to different channels when generating
template (currently not supported by any EQcorrscan functions), then picks
generated here will not give the correct location.

Advanced Example: Parkfield 2004
--------------------------------

.. literalinclude:: ../../tutorials/lag_calc.py
