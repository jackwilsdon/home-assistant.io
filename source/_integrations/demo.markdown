---
title: Demo
description: Instructions on how to use the Platform demos with Home Assistant.
ha_category:
  - Other
  - Update
ha_release: 0.7
ha_quality_scale: internal
ha_codeowners:
  - '@home-assistant/core'
ha_domain: demo
ha_iot_class: Calculated
ha_platforms:
  - air_quality
  - alarm_control_panel
  - binary_sensor
  - button
  - calendar
  - camera
  - climate
  - cover
  - date
  - device_tracker
  - event
  - fan
  - geo_location
  - humidifier
  - light
  - lock
  - media_player
  - notify
  - number
  - remote
  - select
  - sensor
  - siren
  - stt
  - switch
  - text
  - time
  - tts
  - update
  - vacuum
  - water_heater
  - weather
ha_integration_type: integration
---

The `demo` platform allows you to use integrations which are providing a demo of their implementation. The demo entities are dummies but show you how the actual platform looks like. This way you can run own demonstration instance like the online [Home Assistant demo](/demo/) but combined with your own real/functional platforms.

Available demo platforms:

- [Air Quality](/integrations/air_quality/) (`air_quality`)
- [Alarm control panel](/integrations/alarm_control_panel/) (`alarm_control_panel`)
- [Binary sensor](/integrations/binary_sensor/) (`binary_sensor`)
- [Button](/integrations/button/) (`button`)
- [Calendar](/integrations/calendar/) (`calendar`)
- [Camera](/integrations/camera/) (`camera`)
- [Climate](/integrations/climate/) (`climate`)
- [Cover](/integrations/cover/) (`cover`)
- [Device Tracker](/integrations/device_tracker/) (`device_tracker`)
- [Fan](/integrations/fan/) (`fan`)
- [Geolocation](/integrations/geo_location/) (`geo_location`)
- [Humidifier](/integrations/humidifier/) (`humidifier`)
- [Image Processing](/integrations/image_processing/) (`image_processing`)
- [Light](/integrations/light/) (`light`)
- [Lock](/integrations/lock/) (`lock`)
- [Mailbox](/integrations/mailbox/) (`mailbox`)
- [Media Player](/integrations/media_player/) (`media_player`)
- [Notification](/integrations/notify/) (`notify`)
- [Number](/integrations/number/) (`number`)
- [Remote](/integrations/remote/) (`remote`)
- [Select](/integrations/select/) (`select`)
- [Sensor](/integrations/sensor/) (`sensor`)
- [Siren](/integrations/siren/) (`siren`)
- [Switch](/integrations/switch/) (`switch`)
- [Text](/integrations/text/) (`text`)
- [Text-to-speech](/integrations/tts/) (`tts`)
- [Update](/integrations/update/) (`update`)
- [Vacuum](/integrations/vacuum/) (`vacuum`)
- [Water Heater](/integrations/water_heater/) (`water_heater`)
- [Weather](/integrations/weather/) (`weather`)

To integrate a demo platform in Home Assistant, add the following section to your `configuration.yaml` file:

```yaml
# Example configuration.yaml entry

# To load all:
demo:

# To load for a specific integration:
light:
  - platform: demo
```

{% configuration %}
"[component]":
  description: The name of the integration as stated in the listing above the configuration example.
  required: true
  type: string
{% endconfiguration %}
