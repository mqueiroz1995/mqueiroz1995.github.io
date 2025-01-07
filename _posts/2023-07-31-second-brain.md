---
title: Link Blog
date: 2023-07-03 23:00:00 -0300
categories: [second-brain]
tags: [software_engineering]
pin: true
---

Once in a while I fall into the rabbit hole of trying to find content that I've seen in the past. This page tries to collect those golden nuggets somewhere I can easily recall afterward.

{% assign posts_by_year = site.data.linkblog | group_by_exp: "post", "post.date | date: '%Y'" | sort: "name" | reverse %}
{% for year in posts_by_year %}
### {{ year.name }}

{% assign sorted_posts = year.items | sort: 'date' | reverse %}
{% for post in sorted_posts %}
#### [{{ post.title }}]({{ post.link }})
<small>{{ post.date | date: "%Y-%m-%d" }} </small>

{{ post.comment }}

{% endfor %}
{% endfor %}

## Previous

#### [Injection Points](https://marcellogalhardo.dev/posts/injection-points/)

#### [droidcon NYC 2017 - Tech Talks for Humans](https://www.youtube.com/watch?v%253Dd5HYGu_UBNo)

#### [Becoming A Successful Android Open-Source Librarian](https://proandroiddev.com/becoming-a-successful-open-source-librarian-3a008b50b808)

#### [Demystifying the ANRs Puzzle](https://www.amanjeet.me/demystifying-the-anrs-puzzle/)

#### [Herding Elephants - Wrangling a 3,500-module Gradle project](https://developer.squareup.com/blog/herding-elephants/)

#### [The Age of the Essay](http://www.paulgraham.com/essay.html)

#### [Modelling UI State on Android](https://lordraydenmk.github.io/2021/modelling-ui-state/)

#### [Let me write your networking code](https://www.droidcon.com/2019/04/19/let-me-write-your-networking-code/?video%253D334638371)

#### [Dependency Analysis Gradle Plugin: What's an ABI?](https://dev.to/autonomousapps/dependency-analysis-gradle-plugin-what-s-an-abi-3l2h)

#### [Hold on ✋🏻 Before you Dagger or Hilt! Try this Simple DI](https://proandroiddev.com/hold-on-before-you-dagger-or-hilt-try-this-simple-di-f674c83ebeec)

#### [Attacking Build Times With Sample Apps](https://cashapp.github.io/2020-08-25/attacking-build-times-with-sample-apps)

#### [Is High Quality Software Worth the Cost?](https://martinfowler.com/articles/is-quality-worth-cost.html)

#### [Unit Testing, Principles, Practices and Patterns](https://www.amazon.com/Unit-Testing-Principles-Practices-Patterns/dp/1617296279)

#### [Mocks Aren't Stubs](https://martinfowler.com/articles/mocksArentStubs.html)

#### [Android Feature Development at Babylon Health](https://medium.com/babylon-engineering/android-feature-development-at-babylon-health-part-1-thinking-about-the-problem-d1b68521350c)

#### [Let a 1,000 flowers bloom. Then rip 999 of them out by the roots.](https://gigamonkeys.com/flowers/)

#### [Death, Taxes, and HTTP](https://www.youtube.com/watch?v%253D6uroXz5l7Gk)

#### [Shape Up - Stop Running in Circles and Ship Work that Matters ](https://basecamp.com/shapeup)

#### [Surfacing Hidden Change to Pull Requests](https://developer.squareup.com/blog/surfacing-hidden-change-to-pull-requests/)

#### [Growing Object-Oriented Software, Guided by Tests](https://www.amazon.com/Growing-Object-Oriented-Software-Guided-Tests/dp/0321503627)

#### [Test Driven Development: By Example](https://www.amazon.com/Test-Driven-Development-Kent-Beck/dp/0321146530)

#### [Code Complete: A Practical Handbook of Software Construction, Second Edition](https://www.amazon.com/Code-Complete-Practical-Handbook-Construction/dp/0735619670)

#### [The Pragmatic Programmer: From Journeyman to Master](https://www.amazon.com/Pragmatic-Programmer-Journeyman-Master/dp/020161622X)

#### [Clean Code: A Handbook of Agile Software Craftsmanship](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882)
