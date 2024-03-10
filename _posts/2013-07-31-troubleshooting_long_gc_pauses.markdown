---
layout: post
title: "Reducing java microservice resources by 5 times with GraalVM AOT Compilation"
date: 2024-03-10
description: # Microservice in java 
img:  long_gc_pauses.png 
fig-caption: # Add figcaption (optional)
tags: [GraalVM,AOT,JAVA]
---

Java based microservice consumes lot of resources.
This is because running java microservice require jvm and full OS supporting
JVM installation .
### Solution

GraalVM compiler technology can help in reducing the resource as 
it compiles the java byte code to binary format at the build time.
We dont need JVM at run time and it can be run with scratch container image 
if linked statically.

