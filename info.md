In order to get that module running you must ensure that the deconditions are fulfilled.

So the first one:
Running a Alarm System as Runner 8/16
Connected to that system an IP Module running Firmware Ver 2.10.3628 2017 Oct 20 09:48:43
Not connected ANY SSH connection to SSH port 5002

Running Home Assistant higer then Version 0.113

An setup example is given below

crowipmodule:
  host: 10.0.0.xx ( any IP adress it is recommanted to set a static IP adress)
  port: 5002
  keepalive_interval: 60
  timeout: 20
  areas:
    1:
      name: 'Home'  (Name it you like)
    2:
      name: 'None'
      code: '1234'  (Keypad Arm and Disarm Code (User code))
  outputs:
    3:
      name: 'Main Router'
    4:
      name: 'USV Restart'
  zones:
    1:
      name: 'Entrance'
      type: 'motion'
    2:
      name: 'Terrace'
      type: 'door'
    3:
      name: 'Kitchen Window'
      type: 'window'
    4:
      name: 'Kitchen Door'
      type: 'door'
    5:
      name: 'Kitchen Motion'
      type: 'motion'
    6:
      name: 'Bedroom Motion'
      type: 'motion'
    7:
      name: 'Child Room'
      type: 'door'
    8:
      name: 'Child Window Wireless'
      type: 'window'
    9:
      name: 'Child PIR'
      type: 'motion'
    10:
      name: 'Den Motion'
      type: 'motion'
    11:
      name: 'Guest Motion'
      type: 'motion'
    12:
      name: 'Hall Motion'
      type: 'motion'
    13:
      name: 'Hobby Motion'
      type: 'motion'
    14:
      name: 'Bedroom Door'
      type: 'door'
    15:
      name: 'Guest Door'
      type: 'door'
    16:
      name: 'Exit Wireless'
      type: 'door'
