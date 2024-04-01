---
title: "TuYa ZG-205Z control via MQTT"
description: "Integrate your TuYa ZG-205Z via Zigbee2MQTT with whatever smart home infrastructure you are using without the vendor's bridge or gateway."
addedAt: 2023-08-19T9:25:00
pageClass: device-page
---

<!-- !!!! -->
<!-- ATTENTION: This file is auto-generated through docgen! -->
<!-- You can only edit the "Notes"-Section between the two comment lines "Notes BEGIN" and "Notes END". -->
<!-- Do not use h1 or h2 heading within "## Notes"-Section. -->
<!-- !!!! -->

# TuYa ZG-205Z/A

|     |     |
|-----|-----|
| Model | ZG-205Z/A  |
| Vendor  | TuYa  |
| Description | Mini 24Ghz human presence sensor |
| Exposes | Presence, illuminance, Motion state, Large motion detection distance,Large motion detection sensitivity, Small motion detection distance,Small motion detection sensitivity,Static detection distance,Static detection sensitivity,Fading_time,indicator,linkquality |
| Picture | ![TuYa ZG-205Z/A](https://www.zigbee2mqtt.io/images/devices/ZG-205Z-A.jpg) |


<!-- Notes BEGIN: You can edit here. Add "## Notes" headline if not already present. -->
## Notes

### Pairing
To start pairing, press the button (pinhole on the side of the device) using a
pin/paperclip for approx. 5 seconds. The led will turn on, then start blinking while the
pairing process is in progress.
<!-- Notes END: Do not edit below this line -->



## Exposes

### Presence (binary)
Indicates whether the device detected presence.
Value can be found in the published state on the `presence` property.
It's not possible to read (`/get`) or write (`/set`) this value.
If value equals `true` presence is ON, if `false` OFF.

### Motion state (enum)
Indicates the motion state detected by the device (large movements, small movements, static).
Value can be found in the published state on the `Motion state` property.
It's not possible to read (`/get`) or write (`/set`) this value.
If value equals 0:'none', 1:'large', 2:'small', 3:'static'

### Illuminance (numeric)
Raw measured illuminance.
Value can be found in the published state on the `illuminance` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The unit of this value is `lx`.

### Large motion detection distance (numeric)
Value can be found in the published state on the `large_motion_detection_distance` property.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"large_motion_detection_distance": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `10`.
The unit of this value is `m`.

### Large motion detection sensitivity (numeric)
Value can be found in the published state on the `large_motion_detection_sensitivity` property.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"large_motion_detection_sensitivity": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `9`.The higher the value, the more sensitive it is.

### Small motion detection distance (numeric)
Value can be found in the published state on the `small_motion_detection_distance` property.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{small_motion_detection_distance": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `6`.
The unit of this value is `m`.

### Small motion detection sensitivity (numeric)
Value can be found in the published state on the `small_motion_detection_sensitivity` property.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"small_motion_detection_sensitivity": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `9`. The higher the value, the more sensitive it is.

### Static detection distance (numeric)
Value can be found in the published state on the `static_motion_detection_distance` property.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"static_motion_detection_distance": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `6`.
The unit of this value is `m`.

### Static detection sensitivity (numeric)
Value can be found in the published state on the `static_detection_sensitivity` property.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"static_detection_sensitivity": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `9`. The higher the value, the more sensitive it is.


### Fading_time (numeric)
Fading time.
Value can be found in the published state on the `fading_time` property.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"fading_time": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `3600`.
The unit of this value is `s`.

### Indicator (binary)
You can turn the indicator on or off
Value can be found in the published state on the `indicator` property.
It's possible to read (`/get`) or write (`/set`) this value.
If value equals `true` presence is ON, if `false` OFF.

### Linkquality (numeric)
Link quality (signal strength).
Value can be found in the published state on the `linkquality` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The minimal value is `0` and the maximum value is `255`.
The unit of this value is `lqi`.
