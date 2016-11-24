---
title: Mouse and keyboard drivers
company: Screenhero
order: 50
---

As my first task as Screenhero, I refactored the keyboard and mouse drivers. At a very low level, Screenhero modifies, and in some cases completely overrides, the USB input system on Mac. I refactored our drivers to support international keyboards, and the mouse drivers to accurately reflect the user’s designated acceleration curves so that virtual input devices driven by remote users looked and behaved just like locally attached input devices. 