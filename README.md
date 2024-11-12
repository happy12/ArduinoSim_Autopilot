# Sim_Autopilot
Autopilot hardware for flight simulator.

The hardware consist of:
 - one PCB to hold the switches and encoders
 - one PCB to interface between the "Switch PCB" and communications with the PC, using ATMEGA32U4 with USB integration
 - Enclosure that can be 3D printed. Enclosure footprint fits into a RealSimGear cutout for a similar autopilot unit.
 - Integrates with Mobiflight, or one can write their own firmware with Arduino IDE or PlatformIO

Overall the autopilot unit ressemble the Garmin GFC500 and has these buttons:
- HDG, to activate the Heading mode
- APR, to activate the Approach mode
- NAV, to activate the NAV mode (typically VOR or GPS)
- TRK, to activate the Track intercept mode
- AP, to activate the Autopilot mode
- FD, to activate the Flight Director mode
- LVL, to activate the Level mode
- YD, to activate the Yaw Damper mode
- IAS, to activate the "Indicated Airspeed" mode (typically used in climb)
- VNAV, to activate the vertical navigation mode (the vertical guidance on a LNAV approach)
- VS, to activate the Vertical Speed mode (typically used in descent)
- ALT, to activate the Altitude mode

  Encoders typically performs these actions:
  - HDG/TRK: adjust change the heading bug. Pressing the knob synchronize the bug to the current heading
  - ALT SEL: adjust the altitude bug. Pressing the knob synchronize the bug to the current altitude
  - Wheel: adjust the vertical speed when in VS mode, or the indicated airspeed with in IAS mode
 

![Sample Image 1](https://github.com/happy12/Sim_Autopilot/blob/main/CAD_assembly_front.png)
