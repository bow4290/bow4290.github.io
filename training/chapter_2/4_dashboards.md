# 4290 Programming Training Ch 2.4 - Dashboards
## About Dashboards
Dashboards are a vital part of driving & debugging robots. Dashboards are a type of application that runs on the computer running the robot, which provides info about the current state of the robot. When it comes to dashboards, the default one built into WPILib is called SmartDashboard. It is relatively stable and can do most things you need, however it's major shortcoming is how outdated it looks and feels to use. The other official alternative for this is ShuffleBoard, which is significantly more modern in looks, and also provided more features than SmartDashboard. Despite this, ShuffleBoard has a few issues, mainly with stability.

### Presenting Notes
- Dashboards
  - Software that displays information on the current state of the robot
  - Multiple different options, some official, some not.
- SmartDashboard
  - Officially Supported
  - Stable
  - Outdated
- ShuffleBoard
  - (Somewhat) Officially Supported
  - Has potential memory leaks
  - More features, newer look

## Using SmartDashboard and ShuffleBoard
SmartDashboard and ShuffleBoard use essentially\* the same API in WPILib, so anything made for SmartDashboard will work with Shuffleboard, however not vice versa. <br>
*\*For basic usage, they are compatible, but ShuffleBoard has some features that SmartDashboard doesn't*

Since there is a lot to the dashboards, this book wont be going over specific articles, instead, if you would like to learn more I suggest reading the official WPILib articles for both:
- [SmartDashboard Article (WPILib)](https://docs.wpilib.org/en/stable/docs/software/dashboards/smartdashboard/index.html)
- [ShuffleBoard Article (WPILib)](https://docs.wpilib.org/en/stable/docs/software/dashboards/shuffleboard/index.html)

## Unofficial Dashboards
As well as the official dashboards supported by WPILib, there are also other unofficial ones, and a team could even make their own dashboard, following the proper guidelines. One of these dashboards is called Elastic, and is a modern ShuffleBoard alternative made by Team 353. The info for Elastic can be found here:
- [Elastic Dashboard GitHub Repo (Gold872)](https://github.com/Gold872/elastic-dashboard)
- [Elastic Dashboard Wiki (Gold872)](https://github.com/Gold872/elastic-dashboard/wiki)

---

### [<< Previous](./3_joysticks_controllers.md) | Next (Coming Soon...)