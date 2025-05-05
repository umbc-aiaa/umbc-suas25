---
menus:
    main:
        parent: Development
Title: Electronics
---

# Introduction

When selecting electronic components for our plane, we wanted to make sure that they worked over the entire range of the flight while also being easy to configure. When selecting our motors, we wanted to optimize both power and range. Therefore, we focused on having reliable testing infrastructure in this competition year.


# Requirements

For our plane this year, we realized that it would be easier to select our avionics components like servos and other sensors first, and select a flight controller(FC) that supports all of our required equipment on the plane. Therefore, we first brainstormed a list of components we wanted the FC to support which included:

```
- ELRS Reciever
- Telemetry Radio
- GPS
- Object avoidance electronics
- Landing electronics
- Controls surface servo ports
    - Aileron
    - Flaps
    - Tails
- Steerable landing gear
- Kill Switch
- Throttle
- FPV Camera
- Airspeed Sensor(s)
```

We also wanted our FC to be price-efficient, so we considered several options that fit our general requirements:

```
- Pix32 v6
- Holybro Pixhawk4
- Pixhawk 6C
- Kakute H743 Wing
- iFlight BLITZ Wing H743
- Mateksys H743-Wing
- SpeedyBeeF405WING
```

We ended up choosing the Mateksys H743-Wing for its wide availability of ports for the aforementioned requirements, and its great compatibility with Ardupilot.

