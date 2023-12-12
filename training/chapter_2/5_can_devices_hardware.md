# 4290 Programming Training Ch 2.5 - CAN Devices & Hardware
## Motors & Pneumatics
Motors are a invaluable component in building your robot, as they are one of the few ways to add movement. In FRC, these motors are programmed and controlled by attaching motor controllers, although some motors have these built in. Pneumatics are another option for adding a more specific type of movement, as they use pressurized air to move components. Below are some article(s) that explain these components better:
- [1. Article - Beginner Motors (Spectrum 3847)](https://docs.google.com/presentation/d/e/2PACX-1vQx1bBy1RHAYv5y5O5y82e4a45j5DCRmNrwY-d_eOVz8wqks7ehSpiql-qweDWE0J3zzcqMG-5X805x/pub?start=false&loop=false&delayms=3000#slide=id.g9d51526672_0_393)
- [2. Article - Intro to Pneumatics (Spectrum 3847)](https://docs.google.com/presentation/d/1thkZCVNKfHDGw6_co2KAN7cajhKEGYDX1tCw2e6pwqM/edit#slide=id.p)
- [3. Article - Hardware Component Overview (WPILib)](https://docs.wpilib.org/en/stable/docs/controls-overviews/control-system-hardware.html#)

## CAN Devices & Hardware APIs
CAN is a way of connecting robot wires used in FRC. It uses a chain of wires connecting each device, meaning shorter wiring since devices don't have to be individually wired to the roboRIO. CAN devices generally have their own helper WPILib classes, allowing them to be programmed much easier. There are also PWM Motor Controllers, which are controlled roughly the same way as CAN, but connect directly to the roboRIO. The following article explains a basic use case for Motor Controllers:
- [Using Motor Controllers in Code (WPILib)](https://docs.wpilib.org/en/stable/docs/software/hardware-apis/motors/using-motor-controllers.html)

Since there are so many different components and motors that are changing quite frequently, the best way to find out more about these would be to go to the specific documentation for any given motor or component. Below are two articles by WPILib that can help you find the APIs for components:
- [Third-Party CAN Devices (WPILib)](https://docs.wpilib.org/en/stable/docs/software/can-devices/third-party-devices.html)
- [Sensors (WPILib)](https://docs.wpilib.org/en/stable/docs/software/hardware-apis/sensors/index.html)


---

### [<< Previous](./4_dashboards.md) | Next (Coming Soon...)