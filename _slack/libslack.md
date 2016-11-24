---
title: libslack
company: Slack
link: https://slack.engineering/making-slack-feel-like-slack-a7c4e9b6d4fb#.vqzv3gryq
order: 60
---

Previously, our three mobile clients (iPhone, Android, Windows Phone) were entirely siloed projects. I was given the task of architecting a solution to maximize code-sharing between these three platforms. My solution was a cross-platform library in portable C++11, using [djinni](https://github.com/dropbox/djinni) to autogenerate the platform-specific bindings. I was the project lead, responsible for architectural and technical decisions, as well as implementation.