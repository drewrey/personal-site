---
layout: post
title:  "Protocol for WIP PRs"
date:   2018-01-27 00:30:00
category: blog
tags: code-review, protocols
---

version 0.0.1


The Submitter:
- MUST not be done with the work
- SHOULD have the core functionality working
- SHOULD have a list of TO-DO’s that indicate what is required to transition the PR from WIP to “ready”
- CAN present a list of requests for feedback (usually: the core functionality)
- CAN request feedback on particular areas above and beyond the core functionality


The Reviewer:
- SHALL scope the review to the scope presented by the Submitter for feeback
- SHALL assume that a final review will be required once the PR is no longer in WIP status
- CAN request additional changes that are not referenced in the TO-DO’s
- SHALL NOT nit-pick on details relating to style or test failures assuming such issues are properly covered by integration tests and incorporated into a regular PR build pipeline.


The system in which the Submitter/Reviewer reside:
- SHOULD maintain state throughout the review cycle.
- SHOULD make TO-DO requests submitted by the Submitter throughout the process transparent post-hoc, so that follow-up may be verified by final reviewers

