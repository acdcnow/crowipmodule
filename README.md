# crowipmodule
For Crow Runner 16 with IP Module and special Firmware running via SSH
Running in Home Assistant Version 0.113 and higer

Ensure that your Crow Runner IP Module is running the correct firmware.
The standard firmware from Crow or AAP will NOT work!!


configuration settings see configruation.YAML setup

Changelog:
v.0.26 TODO (NOT DONE YET)
- When connection goes off; change all entities to 'unavailable'.
- When HA restarts; update all entities just after the connection is established.
- Check network disconnects real-time.

v.0.25.A
- SwitchDevice, BinarySensorDevice and AlarmControlPanel is deprecated, 
- modify to extend SwitchEntity, BinarySensorEntity and AlarmControlPanelEntity
- Add the respository to HACS

v.0.25
- Corrected HA 103 breaking changes made on alarm_control_panel.
- Outputs controlling and status corrected.

v.0.24
- Removed sensor.area_a_keypad and added sensor.crow_alarm_system; this new sensor has all system related attributes only.
- Handle trigger based disconnection issue.
- Corrected some issues.

v.0.23
- Corrected deepcopy dict, which results area_keypad device attributes to be the same as alarm_control_panel.
- Corrected alarm trigger updates of both area_keypad and alarm_control_panel.

v.0.22
- System binary sensors are converted to alarm control panel device attributes.
- If 'code' configuration is missing in configuration.yaml, then keypad is on in Alarm Panel.
- 'code' configuration is moved to 'areas' section for area specific code.
- Corrected some errors.









