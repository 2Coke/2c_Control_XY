# 2c_Control_XY

## Version 0.0.0

- Added a MultiBall control
- Added a Fader control for changing the ball friction
- Added CustomButton controls for adding and removing balls, for toggling the axis holds as well as for toggling the grid

## Version 0.1.0

- Moved all controls to a tabbed Container and added a Setup tab
- Added a Menu control to Setup tab for selecting the MIDI channel

## Version 0.2.0

- Fixed all MIDI targets should inherit from project MIDI target
- Added CustomButton controls to Setup tab for selecting the X/Y grid sizes as well as Text controls for displaying them respectively

## Version 0.3.0

- Added a Menu control to Setup tab for selecting the MIDI target
- Implemented frame based MIDI send for MultiBall

## Version 0.4.0

- Added CustomButton controls to Control XY tab for forcing the friction fader to min and max position
- Added CustomButton controls to Setup tab for setting the attraction, friction and speed of the friction fader as well as Text controls for displaying the respective values
- Fixed an issue with Lemur where expression handlers were executed on load by implementing a timeout based isLoaded flag

## Version 0.5.0

- Added a Fader control to Control XY tab for changing the ball speed
- Added a CustomButton control to Setup tab for setting the MultiBall attraction value as well as a Text control for displaying it
- Added CustomButton controls to Setup tab for setting the min and max friction and speed values as well as Text controls for displaying them respectively
- Added CustomButton controls to Setup tab for setting the attraction, friction and speed of the speed fader as well as Text controls for displaying them respectively
- Fixed floating point values can not be set to their exact integer pendant (e.g. 0.0 or 1.0)
- Fixed friction fader does not handle min and max values correctly for values other than 0.0 or 1.0
- Refactored object identifiers, improved and cleaned up scripts and added some comments to the code

## Version 0.6.0

- Added a MIDI tab
- Added Knob controls to MIDI tab for defining the MIDI value scale (0-127) per ball and axis as well as Monitor controls for displaying the respective values
- Added CustomButton controls to MIDI tab for resetting the knob values to 0/127 per ball
- Added a CustomButton control for enabling MIDI sends when adjusting the knobs
- Added an array expression to project for defining the MIDI CCs per ball and axis
- Added Monitor and Text controls to MIDI tab for displaying the MIDI CCs per ball and axis
- Added version, copyright and license information to Setup tab
- Added a Text control to Setup tab with a notice about property and attribute values
- Added a Text control to MIDI tab with a notice about how to change MIDI CCs

## Version 0.7.0

- Created a generic Container with CustomButton controls for incrementing and decrementing arbitrary properties or attributes, a Monitor control for displaying the respective value as well a Text control as label
- Updated all Setup tab control groups based on the generic Container
- Updated all MIDI tab knob controls with expression instead of frame based MIDI sends
- Added a Container as splash screen and moved version, copyright and license information Text controls from Setup tab to the splash screen
- Added Text and Monitor controls to splash screen to show load progress as percentage
- Adjusted incremental/decremental steps for ball speed +/- controls at Setup tab from 0.5 to 0.1 for the range between -1.0 and 1.0

## Version 0.7.1

- Fixed friction min/max and speed min/max values can not be saved

## Version 0.8.0

- Added control groups to MIDI tab for configuring the MIDI CCs per ball and axis
- Added a Text control to MIDI tab with a notice about rounding deviation
- Removed a Text control from MIDI tab which contained a notice about how to change MIDI CCs

## Version 0.9.0

- Changed project skin to "Classic"
- Adjusted MIDI tab knobs friction to 1.0
- Created a GitHub repository with jzml project file, CHANGELOG.md, LICENSE.md and README.md as well as an Ableton Live project for testing and demonstration purposes

---

## Backlog / Roadmap

- Implement bi-directional MIDI message support (receiving X/Y values should force all balls to stop immediately)
