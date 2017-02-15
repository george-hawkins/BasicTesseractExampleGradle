# BasicTesseractExampleMaven

This is a fork of [piersy](https://github.com/piersy)'s [BasicTesseractExampleGradle](https://github.com/piersy/BasicTesseractExampleGradle) project that has been modifed so that it can be built with Maven rather than Gradle.

The included test [`BasicTesseractExampleTest`](https://github.com/george-hawkins/BasicTesseractExampleMaven/blob/master/src/test/java/BasicTesseractExampleTest.java) demonstrates how simple it is to use [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) from Java.

Clone this repository, set the `os.classifier` property (see below) and then run the following - if the test succeeds you should see the text "This is a lot of 12 point..." printed to the console.

```
$ mvn clean test
```

**Important:** you need to modify the value of the `os.classifier` property in [`pom.xml`](pom.xml) to match the operating system you are using:
```XML
<!-- Valid classifiers for javacpp-presets are android-arm, linux-ppc64le, linux-x86, macosx-x86_64 and windows-x86. -->
<os.classifier>macosx-x86_64</os.classifier>
```
By default it is set to `macosx-x86_64` (as shown).
