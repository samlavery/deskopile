# Deskopile
Real human presence detection, effortless project time tracking, and a built in child silencer.  Everything needed for the modern remote worker. 


## Why The World Needs This Project 
As the great Larry Wall once said, amongst engineers, laziness is a virtue.  When it comes to things like tracking time for project billing and tps reports, I'm as lazy as they come.  I'm also constantly running late to meetings because I'm usually so deep into a problem space that no blinking notification will pull me out.  Finally, like everyone else, I currently work from home... with kids... every... single.... day.  I don't know about your children, but mine like to burst into the room screaming during conference calls.  Deskopile to the rescue!

## Current Components
* Omron D6T Thermopile Sensor
* Arduino Based - Atmel 2560 - NodeMCU 8266
* 3.5 inch TFT LCD screen
* Spare PC running Linux & pgsql & tsbd 
* Local ThingsBoard IoT Server (testing)
* Server side module for custom logic
* A wireless network
* Jumpers/resistors/solder/misc electronic parts


## Features
#### Time Tracking and Reporting
Even today, it's not exactly easy for electronics to accurately tell if a person in front of them or not.  Previously, this was done using PIR sensors, but unfortunately for the sedentary engineer, this isn't a viable solution.  Along came the Thermopile sensor, which you should research if you don't know about yet.  They are fascinating little pieces of technology that measure the temperature of the things in front of it compared to an internal refernence ambient temperature.  They do this using the same principal as old metal thermometers, two materials react differently to temperature and that difference is measured and translated into a digital output.  In this case, you get an 8x8 grid (64 pixels) of predator style thermoptic vision.  For me, I have a workstation that I sat at and only do work there.  I do general internet surfing/gaming elsewhere in the house. So, if I can reliable measure and track when I am sitting in the chair, I can build something to track my hours worked on various projects without any effort at all. I plan on creating some nice visualizations for this as well.

#### Personal Assistant
My life is complex, I have a wife, kids, like 8 bosses, and a million things to do.  I am constantly 3-5 minutes late to meetings because I'm also solving insanely complicated problems in addition to everything else.  Deskopile will act as a point of aggregation for all my various appointments/schedules/reminders and to-do's, privately.  With that knowledge, I shall attempt to extract actionable notifactions that work.  I hope to avoid any form of ML, but we shall see. 


#### Child Silencer

Everyone with children who works remotely has at one point had them burst into the room screaming about candy, video games, being pinched, and/or nothing at all, at exactly the wrong moment during your team's daily standup call.  Deskopile will teach my children that a green light means it's ok to come in screaming and a red light means be quiet....or else.  V1 is using the TFT screen as an indicator, in the future we may need to remote control external lights (outside the door).  


## Future Roadmap
* Large and solid tactile switches
* Automatic call detection... somehow?
* Personal scheduler integration
* Something that makes coffee
* A case
* Ideas?





## Status
prototyping....

I was able to get D6T wired up with pulldown resistors on a breadboard connected via I2C to the mega 256!  It worked the first time amazingly.  The sensor appears to read ambient at 60F, clothing at 80F, and skin at about 90F, these are numbers we can work with!  So far so good!  But I need go back and rewire things up properly before moving on to the next steps.

More to come.

