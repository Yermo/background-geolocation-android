# Project Notes

## src/test

Unit tests that can run on the host JVM.

## src/androidTest

"intrumented tests" that run on an Android Device. When right clicking on any test in this folder
a modal will appear asking for the device to run the tests on.

## src/main

The main source project directory

### src/main/java/com

The source of this project.

### src/main/preoreo and src/main/oreo

Apparently some differences in versions of Android oreo and pre-oreo.

Oreo is Android API Level 26

### src/main/java/org

Apparently some code borrowed from the apache and chromium projects.

#### src/main/java/org/apache

I'm not sure if ReversedLinesFileReader is used anywhere.

#### src/main/java/org/chromium

ThreadUtils is used in LocationServiceImpl.java

## src/main/java/ru

An sqlbuilder and some utilities.
