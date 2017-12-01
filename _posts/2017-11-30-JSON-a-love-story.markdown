---
layout: post
title:  "JSON - a love story"
date:   2017-11-30 11:50:00
category: blog
tags: TIL, json
---

Scene: adding a PUT route with a `bodyParser.json()` as middleware.

- Creates request in Postman as application/json
> GetSyntaxError: Unexpected token \"\n

- Uncertain, tries a few other things (removing middleware, using `debugger` statements, ...)

- Those being unsuccessul, decides to validate request body
- Gets:
> :warning: Error:Strings should be wrapped in double quotes.[Code 17, Structure 2]

- :open_mouth:
- `:%/s/\'/\"/g`
- ...
- PUT route now works! :tada:

TIL: json expects `"` and not `'`
