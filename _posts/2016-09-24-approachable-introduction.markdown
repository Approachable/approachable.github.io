---
layout:     post
title:      "Introduction to Approachable for Developers and Makers"
date:       2016-10-14 12:00:00
author:     "Approachable"
---

> We are stuck with technology when what we really want is just stuff that works. -- Douglas Adams, The Salmon of Doubt

Not long ago, I bought a major brand camera that had two new features that appealled to me. One feature, was Wifi. I thought it would be really great to automatically upload picture to online services. The other feature was Near Field Communication (NFC). I had experimented with NFC in my own designs and knew how great it was for improving usability. Just consider how much easier it is to perform a Wifi handoff with an NFC phone tap instead of having to type in a network password using a camera button pad.

You can imagine my surprise when I found that the only function that the NFC served was to automate the starting of the manufacturers smart phone app. Thinking this could not possible be right, I spent 30 minutes looking through the manual in order to verify this limitation. I felt dissappointed and frustrated that I had wasted so much of my time on such a useless feature. It did get me wondering however...When we fail to present users with a consistent value proposition for using a technology like NFC, do we train them to ignore it in the future?

# Purpose

We all have experiences like this. We waste too much of our lives fidgeting with technology that does not offer a quality user experience. Approachable's purpose is to get the user experience right by creating a Walk-Up-And-Use Framework that can be employed with most everyday electronics.

# How It Works For Users (3 simple steps)

1. Users begin interaction in one of two ways:
        
    a. The device uses NFC: the user puts their phone very close to the product and the device is identified
    
    b. The device uses Bluetooth Low Energy (BLE): All nearby devices appear in the Android notifications menu and the user selects the device of interest
2. The user is shown relevant device information including current status, configuration apps, and Help related content
3. The user changes the configuration using the app:
    
    a. With NFC devices, the user touches the phone to device to write the changed settings
    
    b. For BLE devices, the changed settings take place immediately

# How It Works for Developers/Makers (4 simple steps)

1. Decide whether to use BLE, NFC, or both in your hardware design. We are open sourcing and documenting every demo implementation that we can to make this as easy as possible.

2. Choose what you want to display or configure with the smartphone and create a corresponding [JSON Schema](http://json-schema.org/). e.g. setting Wifi parameters:
```
{
    "type": "object",
    "title": "Wifi Setup",
    "properties": {
        "SSID": {
            "type": "string",
            "title": "Network Name (SSID)"
        },
        "Password": {
            "type": "string",
            "format": "password",
            "title": "Password"
        }
    }
}
```

3. Put your schemas into a manifest on the [Approachable Device Registry](https://apprsand.herokuapp.com) Developer Sandbox. The registry will provide you with an interface identifier that your device will use to identify itself when scanned via NFC.

4. Complete your hardware design by integrating the available example projects and libraries.


