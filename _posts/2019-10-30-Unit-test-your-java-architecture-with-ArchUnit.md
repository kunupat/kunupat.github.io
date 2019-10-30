---
title:  "Test Your Java Architecture with ArchUnit- A Practical Example"
date:   2019-10-30 21:20:50 +0530
---

Testing Java Singleton Design Pattern using ArchUnit.


I recently came across an article about the ArchUnit framework in Java Magazine and it instantly caught my attention. I thought of giving it a try as I am transitioning into Java Architect’s role. Even working as a Technical Lead, I had faced this challenge of ensuring that my team follows the solution architecture and guidelines prescribed to them and the resulting solution actually matches the architecture blueprint. As new developers join a development team or as the application maintenance team adds in fixes and features, they tend to diverge from the original designs over a period. I have also seen that usually, new team members look at the existing codebase to infer the design. And if they look at and follow the diverged part of the code, they will create even messier codebase. Even having software documentation in place, we know for real that there are very few developers who read the documentation and even fewer keep the documentation up-to-date. Also, chances of applying the documented design standards are left to the individuals who maintain the application.
Having had these practical experiences, when I read about ArchUnit, it felt like I found the right solution to the aforementioned problems. As ArchUnit is based on the popular JUnit testing framework, unit testing of architecture can be easily integrated into the existing CI/CD pipelines enforcing the architecture compliance in each release.

Read complete article [here] (https://medium.com/@kunal.m.patil/test-your-java-architecture-with-archunit-a-practical-example-30b2f56046a)

The sample code can be found here- https://github.com/kunupat/singleton
