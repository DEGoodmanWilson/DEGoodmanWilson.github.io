---
title: Slack Calls
company: Slack
link: https://techcrunch.com/2016/03/02/slack-calls
order: 80
---

While part of the Calls team (previously Screenhero), I was responsible for integrating the shared C++ library that Calls is built upon into the Mac, Windows, and Linux desktop Slack clients. On Mac, I chose to use XPC Services for maximum isolation and robustness. The Windows and Linux clients, built using Electron, required a set of V8 bindings to the Calls library.