
# Squandor Home Assistant config files

## Images
### Home page
![home_page](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/raw/branch/master/www/img/home_page.png)

### Sensor page
![sensor_page](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/raw/branch/master/www/img/sensor_page.png)

### Server page
![server_page](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/raw/branch/master/www/img/server_page.png)

### Printer page
![printer_page](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/raw/branch/master/www/img/printer_page.png)

## Noteworthy (useful) automations
See *all* my automations and its dependencies [down the page](#automations---table-of-content)!

## My devices

<!-- start-table -->

<!-- end-table -->

<!-- start-automations -->
# Automations - Table of Content
1. [check_afval_groen ](#check_afval_groen) (4 entities)
1. [Trigger alarm while armed away ](#trigger-alarm-while-armed-away) (4 entities)
1. [update dns record transip ](#update-dns-record-transip) (2 entities)
1. [camera_cast_select_voordeur ](#camera_cast_select_voordeur) (12 entities)
1. [Kitchen Ledstrip Change Color Purple ](#kitchen-ledstrip-change-color-purple) (6 entities)
1. [message if octoprint finished ](#message-if-octoprint-finished) (1 entities)
1. [If its gonna rain ](#if-its-gonna-rain) (4 entities)
1. [Switch gang lampen ](#switch-gang-lampen) (10 entities)
1. [Set HA theme for day and night ](#set-ha-theme-for-day-and-night) (4 entities)
1. [hue dimmer switch woonkamer_on ](#hue-dimmer-switch-woonkamer_on) (12 entities)
1. [Message if memory is above 80% ](#message-if-memory-is-above-80%) (2 entities)
1. [toggle_kas_lamp ](#toggle_kas_lamp) (2 entities)
1. [Nobody Home ](#nobody-home) (5 entities)
1. [Volume Slider change Badkamer ](#volume-slider-change-badkamer) (6 entities)


⚠️ Total number of automations: **74** ⚠️

## [check_afval_groen ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/afval_automations.yaml)
### [check_afval_groen ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/afval_automations.yaml#L1)

  *which uses:*
  - [sensor.afval_groen](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/sensors/template_sensors.yaml#L156)

### [check_afval_restafval ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/afval_automations.yaml#L16)

  *which uses:*
  - [sensor.afval_restafval](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/sensors/template_sensors.yaml#L159)

### [check_afval_papier ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/afval_automations.yaml#L31)

  *which uses:*
  - [sensor.afval_oudpapier](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/sensors/template_sensors.yaml#L153)

### [check_afval_plastic ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/afval_automations.yaml#L46)

  *which uses:*
  - [sensor.afval_plastic](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/sensors/template_sensors.yaml#L162)

[^ toc](#automations---table-of-content)


## [Trigger alarm while armed away ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/alarm_automations.yaml)
### [Trigger alarm while armed away ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/alarm_automations.yaml#L2)

  *which uses:*
  - [group.deur_sensors_gang](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/motion_groups.yaml#L13)
  - [group.motion_woonkamer](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/motion_groups.yaml#L1)

### [Trigger alarm while armed at night ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/alarm_automations.yaml#L21)

  *which uses:*
  - [group.motion_woonkamer](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/motion_groups.yaml#L1)

### [Send notification when alarm triggered ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/alarm_automations.yaml#L40)



### [anet a8 smoke detector ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/alarm_automations.yaml#L49)



[^ toc](#automations---table-of-content)


## [update dns record transip ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/automations.yaml)
### [update dns record transip ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/automations.yaml#L1)

  *which uses:*
  - [script.update_transip](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/scripts/scripts.yaml#L16)
  - [binary_sensor.external_ip_diff](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/binary_sensors/binary_sensors.yaml#L8)

### [Wake Me Up ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/automations.yaml#L18)

  *which uses:*
  - [input_boolean.alarmstatus](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_boolean.yaml#L1)
  - [input_boolean.alarmweekday](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_boolean.yaml#L5)
  - [script.start_spotify_wekker](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/scripts/scripts.yaml#L20)
  - [sensor.alarm_time](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/sensors/template_sensors.yaml#L197)
  - [shell_command.speaker_google_home_slaapkamer_volume_up](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/shell_commands/shell_commands.yaml#L20)

[^ toc](#automations---table-of-content)


## [camera_cast_select_voordeur ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/camera_automations.yaml)
### [camera_cast_select_voordeur ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/camera_automations.yaml#L1)

  *which uses:*
  - [input_select.camera_cast_select](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_select.yaml#L19)

### [camera_cast_select_tuin ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/camera_automations.yaml#L14)

  *which uses:*
  - [input_select.camera_cast_select](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_select.yaml#L19)

### [camera_cast_select_baby ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/camera_automations.yaml#L25)

  *which uses:*
  - [input_select.camera_cast_select](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_select.yaml#L19)

### [send pic on ttgo_motion_dark ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/camera_automations.yaml#L37)



### [send pic on ttgo_motion_light ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/camera_automations.yaml#L83)



### [send pic on ttgo doorbell_overdag ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/camera_automations.yaml#L130)



### [send pic on ttgo doorbell_avond ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/camera_automations.yaml#L193)



### [send picture on doorbell ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/camera_automations.yaml#L253)



### [motion_ttgo_doorbell ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/camera_automations.yaml#L312)

  



### [motion text reset ttgo doorbell ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/camera_automations.yaml#L327)

  



### [webhook endpoint to motion backdoor nas ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/camera_automations.yaml#L346)

  *which uses:*
  - [sensor.backdoor_motion_state](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/sensors/template_sensors.yaml#L211)

### [Webhook endpoint to motion frontdoor nas ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/camera_automations.yaml#L378)

  *which uses:*
  - [sensor.frontdoor_motion_state](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/sensors/template_sensors.yaml#L208)

[^ toc](#automations---table-of-content)


## [Kitchen Ledstrip Change Color Purple ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/led_strip_automations.yaml)
### [Kitchen Ledstrip Change Color Purple ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/led_strip_automations.yaml#L1)

  *which uses:*
  - [input_select.keuken_led_strip](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_select.yaml#L1)
  - [shell_command.kitchen_led_paars](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/shell_commands/shell_commands.yaml#L1)

### [Kitchen Ledstrip Change Color Red ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/led_strip_automations.yaml#L9)

  *which uses:*
  - [input_select.keuken_led_strip](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_select.yaml#L1)
  - [shell_command.kitchen_led_rood](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/shell_commands/shell_commands.yaml#L2)

### [Kitchen ledstrip change color off ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/led_strip_automations.yaml#L17)

  *which uses:*
  - [input_select.keuken_led_strip](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_select.yaml#L1)
  - [shell_command.kitchen_led_off](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/shell_commands/shell_commands.yaml#L6)

### [Kitchen Ledstrip Change Color Green ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/led_strip_automations.yaml#L25)

  *which uses:*
  - [input_select.keuken_led_strip](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_select.yaml#L1)
  - [shell_command.kitchen_led_groen](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/shell_commands/shell_commands.yaml#L3)

### [Kitchen Ledstrip Change Color Blauw ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/led_strip_automations.yaml#L33)

  *which uses:*
  - [input_select.keuken_led_strip](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_select.yaml#L1)
  - [shell_command.kitchen_led_blauw](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/shell_commands/shell_commands.yaml#L5)

### [Kitchen Ledstrip Change Color White ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/led_strip_automations.yaml#L41)

  *which uses:*
  - [input_select.keuken_led_strip](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_select.yaml#L1)
  - [shell_command.kitchen_led_wit](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/shell_commands/shell_commands.yaml#L4)

[^ toc](#automations---table-of-content)


## [message if octoprint finished ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/octoprint_automations.yaml)
### [message if octoprint finished ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/octoprint_automations.yaml#L1)



[^ toc](#automations---table-of-content)


## [If its gonna rain ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/rain_automations.yaml)
### [If its gonna rain ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/rain_automations.yaml#L1)

  *which uses:*
  - [input_select.keuken_led_strip](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_select.yaml#L1)
  - [sensor.old_kitchen_led_color](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/sensors/template_sensors.yaml#L113)
  - [sensor.today_rain_mm](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/sensors/template_sensors.yaml#L70)

### [If rain stops ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/rain_automations.yaml#L21)

  *which uses:*
  - [input_select.keuken_led_strip](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_select.yaml#L1)
  - [sensor.old_kitchen_led_color](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/sensors/template_sensors.yaml#L113)

### [check_garden_water ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/rain_automations.yaml#L32)

  *which uses:*
  - [sensor.today_rain_mm](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/sensors/template_sensors.yaml#L70)

### [check_garden_water_20min ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/rain_automations.yaml#L54)



[^ toc](#automations---table-of-content)


## [Switch gang lampen ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/sensor_automations.yaml)
### [Switch gang lampen ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/sensor_automations.yaml#L1)



### [Turn off light 10 minutes after last movement gang ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/sensor_automations.yaml#L12)



### [trigger_ligts_motion_frontdoor_10_minutes ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/sensor_automations.yaml#L21)

  *which uses:*
  - [sensor.motion_frontdoor_activated](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/sensors/template_sensors.yaml#L182)

### [trigger_lights_motion_door_living_room ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/sensor_automations.yaml#L38)

  *which uses:*
  - [group.deur_sensors_gang](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/motion_groups.yaml#L13)

### [Turn off light 5 minutes after gang_beneden on ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/sensor_automations.yaml#L51)



### [Turn off light 5 minutes after gang_beneden on ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/sensor_automations.yaml#L51)



### [Wasmachine is klaar ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/sensor_automations.yaml#L73)

  *which uses:*
  - [binary_sensor.wasmachine_state](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/binary_sensors/binary_sensors.yaml#L11)

### [Wasmachine gaat weer beginnen ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/sensor_automations.yaml#L89)

  *which uses:*
  - [binary_sensor.wasmachine_state](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/binary_sensors/binary_sensors.yaml#L11)

### [woonkamer motion lights ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/sensor_automations.yaml#L106)

  *which uses:*
  - [group.contacts_woonkamer](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/motion_groups.yaml#L8)
  - [group.motion_woonkamer](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/motion_groups.yaml#L1)

### [turn woonkamer spots off 30 minutes after last movement ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/sensor_automations.yaml#L127)

  *which uses:*
  - [group.motion_woonkamer](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/motion_groups.yaml#L1)

[^ toc](#automations---table-of-content)


## [Set HA theme for day and night ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/sun_automations.yaml)
### [Set HA theme for day and night ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/sun_automations.yaml#L2)



### [run_on_sunset ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/sun_automations.yaml#L17)

  *which uses:*
  - [input_select.keuken_led_strip](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_select.yaml#L1)
  - [group.all_camera_motion](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/camera_groups.yaml#L1)
  - [group.garden_lights](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/light_groups.yaml#L1)

### [run_at_midnight ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/sun_automations.yaml#L34)

  *which uses:*
  - [input_select.keuken_led_strip](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_select.yaml#L1)
  - [group.garden_lights](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/light_groups.yaml#L1)

### [run_at_sunrise ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/sun_automations.yaml#L49)

  *which uses:*
  - [group.all_camera_motion](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/camera_groups.yaml#L1)
  - [group.people](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/person_groups.yaml#L1)

[^ toc](#automations---table-of-content)


## [hue dimmer switch woonkamer_on ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/switches_automations.yaml)
### [hue dimmer switch woonkamer_on ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/switches_automations.yaml#L1)



### [hue dimmer switch woonkamer_off ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/switches_automations.yaml#L14)



### [hue dimmer switch woonkamer_up ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/switches_automations.yaml#L27)

  *which uses:*
  - [group.alle_keuken_lampen](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/light_groups.yaml#L14)

### [hue dimmer switch woonkamer_down ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/switches_automations.yaml#L36)

  *which uses:*
  - [group.alle_keuken_lampen](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/light_groups.yaml#L14)

### [hue dimmer switch slaapkamer_on ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/switches_automations.yaml#L45)

  *which uses:*
  - [group.slaapkamer_lampen](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/light_groups.yaml#L30)

### [hue dimmer switch slaapkamer_off ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/switches_automations.yaml#L63)

  *which uses:*
  - [group.slaapkamer_lampen](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/light_groups.yaml#L30)

### [hue dimmer switch slaapkamer_san_up_on ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/switches_automations.yaml#L81)



### [hue dimmer switch slaapkamer_san_up_off ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/switches_automations.yaml#L94)



### [hue dimmer switch slaapkamer_laris_up_on ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/switches_automations.yaml#L107)



### [hue dimmer switch slaapkamer_laris_up_off ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/switches_automations.yaml#L120)



### [Denon AMP Channel TV ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/switches_automations.yaml#L134)

  *which uses:*
  - [input_select.amp_receiver_input](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_select.yaml#L12)
  - [shell_command.amp_receiver_tv](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/shell_commands/shell_commands.yaml#L8)

### [Denon AMP Channel Airplay ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/switches_automations.yaml#L142)

  *which uses:*
  - [input_select.amp_receiver_input](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_select.yaml#L12)
  - [shell_command.amp_receiver_airplay](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/shell_commands/shell_commands.yaml#L9)

[^ toc](#automations---table-of-content)


## [Message if memory is above 80% ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/systemmonitor_automations.yaml)
### [Message if memory is above 80% ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/systemmonitor_automations.yaml#L1)



### [Message if swap is above 80% ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/systemmonitor_automations.yaml#L11)



[^ toc](#automations---table-of-content)


## [toggle_kas_lamp ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/time_automations.yaml)
### [toggle_kas_lamp ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/time_automations.yaml#L1)



### [Reset power / Gas variables / today_rain ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/time_automations.yaml#L12)

  *which uses:*
  - [input_number.midnight_gas_consumption](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_number.yaml#L58)
  - [input_number.midnight_power_consumption_low](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_number.yaml#L38)
  - [input_number.midnight_power_consumption_normal](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_number.yaml#L42)
  - [input_number.midnight_power_production_low](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_number.yaml#L48)
  - [input_number.midnight_power_production_normal](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_number.yaml#L52)
  - [sensor.today_rain_mm](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/sensors/template_sensors.yaml#L70)

[^ toc](#automations---table-of-content)


## [Nobody Home ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/tracker_automations.yaml)
### [Nobody Home ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/tracker_automations.yaml#L1)

  *which uses:*
  - [group.all_camera_motion](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/camera_groups.yaml#L1)
  - [group.people](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/person_groups.yaml#L1)

### [Something turned on while leaving ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/tracker_automations.yaml#L19)

  *which uses:*
  - [group.alle_keuken_lampen](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/light_groups.yaml#L14)
  - [group.slaapkamer_lampen](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/light_groups.yaml#L30)
  - [group.people](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/person_groups.yaml#L1)

### [Nobody home 10 min. switch tv ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/tracker_automations.yaml#L49)

  *which uses:*
  - [switch.tv_livingroom](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/switches/template_switches.yaml#L31)
  - [group.people](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/person_groups.yaml#L1)

### [Someone Home motion before sunset ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/tracker_automations.yaml#L64)

  *which uses:*
  - [group.all_camera_motion](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/camera_groups.yaml#L1)
  - [group.people](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/person_groups.yaml#L1)

### [Someone home motion after sunset ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/tracker_automations.yaml#L82)

  *which uses:*
  - [group.people](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/groups/person_groups.yaml#L1)

[^ toc](#automations---table-of-content)


## [Volume Slider change Badkamer ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/volume_switches.yaml)
### [Volume Slider change Badkamer ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/volume_switches.yaml#L2)

  *which uses:*
  - [input_number.speaker_badkamer_volume_slider](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_number.yaml#L1)

### [Volume Change Badkamer ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/volume_switches.yaml#L9)

  *which uses:*
  - [input_number.speaker_badkamer_volume_slider](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_number.yaml#L1)

### [Volume Slider change PCSander ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/volume_switches.yaml#L19)

  *which uses:*
  - [input_number.speaker_pcsander_volume_slider](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_number.yaml#L7)

### [Volume Change PCSander ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/volume_switches.yaml#L26)

  *which uses:*
  - [input_number.speaker_pcsander_volume_slider](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_number.yaml#L7)

### [Volume Slider change Woonkamer ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/volume_switches.yaml#L36)

  *which uses:*
  - [input_number.speaker_woonkamer_volume_slider](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_number.yaml#L13)

### [Volume Change Woonkamer ](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/automations/volume_switches.yaml#L43)

  *which uses:*
  - [input_number.speaker_woonkamer_volume_slider](https://git.digitaal-rechercheurs.nl:9090/squandor/homeassistant/src/branch/master/configurations/inputs/input_number.yaml#L13)

[^ toc](#automations---table-of-content)


<!-- end-automations -->