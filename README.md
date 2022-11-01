# TripleBypassV2Plus
A Variant of Tian Feng's Triple Bypass V2 with fixes and functionality added

## Headphone Audio Restoration

### VA3-VA6 (Probably earlier variants as well)
On the bottom of the board under the CXA1034 (or similar) IC, remove:
- C45-C48
- R42-43 (Mono audio amplifier summing resistors)
- R34, 37

The HR pad will then connect to C43-negative and HL will connect to C41 negative.

### VA7
- Remove R29-30 and C19-20 (They are next to IC9, lower left hand corner of the board)
- IC9: Lift pins 8 and 14
- The HR pad will connect to the upper side (facing the AV section) of R46
- The HL pad will connect to the upper side of R45

![VA7 Headphone Amp Connections](/images/Headphone%20Amp%20Connections.jpg)

## CVBS Restoration

These instructions assume the subcarrier pin has not been lifted!
*** Leave the 3BP S75 jumper open (no solder) for Model 2 ***

-Model 1
For models VA3-VA6 (likely earlier models too, unconfirmed), on the bottom side of the board, remove:
R17/19/21 (4.7 kOhm)

Solder:
RO to the empty pad of R17 that has continuity to C25
GO to the empty pad of R19 that has continuity to C26
BO to the empty pad of R21 that has continuity to C27

-Model 1 VA7, Model 2
Remove R62-64

Solder RO to either pad that junctions R58, C25 and R62
Solder GO to either pad that junctions R59, C26 and R63
Solder RO to either pad that junctions R60, C27 and R64

For Model 2 systems, keep Pins 21-23 of the RGB encoder lifted. M1VA7 outputs will be restored to the original DIN and will not impact signals to the 9 Pin DIN.

