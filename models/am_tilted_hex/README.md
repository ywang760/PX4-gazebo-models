# Aerial Manipulator tilted-hex SITL model

This model preserves the compatibility-locked six-motor order, 30-degree
axes, alternating spin directions, measured 7.024 kg as-flown mass, and
measured 0.3683 m rotor radius.

The following values are intentionally simulation surrogates, not identified
hardware parameters:

- diagonal inertia is the planar six-point-ring estimate
  `Ixx=Iyy=m*r^2/2=0.476385 kg m^2`, `Izz=m*r^2=0.952770 kg m^2`;
- each rotor supplies 26.5127 N at 1500 rad/s, giving twice-hover vertical
  authority in aggregate;
- reaction torque uses the historical normalized magnitude `|Km|=0.05`;
- aerodynamic drag constants use the PX4 Gazebo multicopter defaults.

Replace these values only from qualified identification evidence. This model
and its PX4 airframe are SITL-only and do not authorize an FMU build or flash.
