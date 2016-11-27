---
title: Mac desktop realtime video rendering pipeline
company: Screenhero
order: 40
---

Screenhero is screen sharing that is optimized for latency. I was responsible for ensuring that incoming frames are rendered as quickly as possible. I implemented a zero-latency buffering scheme, that fed packets to ffmpeg for decoding, and an OpenCL workflow that allowed us to render directly from the generated YUV frames that was far more efficient that decoding the YUV frames on the CPU.