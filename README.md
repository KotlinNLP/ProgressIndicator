# ProgressIndicator

ProgressIndicator implements different indicators to track a progress: 
* Bar ```|███████████ | 95%```
* Icon ```/``` ```-``` ```\ ``` ```|```
* Percentage ```[60%]```

ProgressIndicator is part of [KotlinNLP](http://kotlinnlp.com/ "KotlinNLP").


## Getting Started

Simply declare a ProgressIndicator passing it the total amount of steps to track and the call the `tick()` method to 
fo forward of one single step. Is it possible to pass it the amount of steps setting the `amount` parameter.
```kotlin
import com.kotlinnlp.progressindicator.ProgressIndicatorBar

val progress = ProgressIndicatorBar(1000)

(0 until 1000).forEach {
  progress.tick()
  Thread.sleep(10)
}
```


## License

This software is released under the terms of the 
[Mozilla Public License, v. 2.0](https://mozilla.org/MPL/2.0/ "Mozilla Public License, v. 2.0")


## Contributions

We greatly appreciate any bug reports and contributions, which can be made by filing an issue or making a pull 
request through the [github page](https://github.com/KotlinNLP/ProgressIndicator "ProgressIndicator on GitHub").