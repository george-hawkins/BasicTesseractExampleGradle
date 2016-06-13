# BasicTesseractExampleMaven

This is a fork of [piersy](https://github.com/piersy)'s [BasicTesseractExampleGradle](https://github.com/piersy/BasicTesseractExampleGradle) project that has been modifed so that it can be built with Maven rather than Gradle.

The included test [`BasicTesseractExampleTest`](https://github.com/george-hawkins/BasicTesseractExampleMaven/blob/master/src/test/java/BasicTesseractExampleTest.java) demonstrates how simple it is to use [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) from Java.

Clone this repository and run the following - if the test succeeds you should see the text "This is a lot of 12 point..." printed to the console.

```
$ mvn clean test
```
