---
layout: post
title: "Kotlin Test"
author: "Andrey Breslav"
categories: journal
tags: [coding,kotlin,android]
image: cutting.jpg
---
This is a post to test kotlin code highlighting

```kotlin
class InitOrderDemo(name: String) {
    val firstProperty = "First property: $name".also(::println)

    init {
        println("First initializer block that prints ${name}")
    }

    val secondProperty = "Second property: ${name.length}".also(::println)

    init {
        println("Second initializer block that prints ${name.length}")
    }
}
```