---
layout: page
title: "Configurator"
description: "Instructions on how to integrate the configurator in your components."
date: 2015-03-15 00:51
sidebar: true
comments: false
sharing: true
footer: true
logo: home-assistant.png
ha_category:
  - Other
ha_qa_scale: internal
ha_release: 0.7
---

<div class='note'>
This integration is intended for developers.
</div>

The configurator integration allows integrations to request information from the user. It is currently implemented as the minimum viable product:

- It supports showing a text, image and button to the user
- Input fields can be defined with a description, and optional type
- It will trigger a callback when the button is pressed

The Hue integration in [the demo](/demo) and Plex are implemented using the configurator. See [the source of the demo integration](https://github.com/home-assistant/home-assistant/tree/dev/homeassistant/components/demo) for a simple example.

See [the source](https://github.com/home-assistant/home-assistant/tree/dev/homeassistant/components/configurator) for more details on how to use the configurator integration.
