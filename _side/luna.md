---
title: Luna
order: 3
link: http://d.e.goodman-wilson.com/luna/
github: luna
---

An embedded HTTP(S) server in modern C++, Luna is designed to be easy to use and integrate with your C++ project.
Server creation, start, shut down, and deletion are all handled behind the scenes with the magic of RAII. Adding
endpoints to your server is likewise meant to be simple. Nominate an endpoint with a string or regex and an HTTP
verb, and pass in a lambda or other `std::functional`-compatible object (function pointers, bound class member functions),
and return a string containing the desired response body. Of course, you can set response codes, headers, and MIME
types, too.
