# Android Browser Helper

![CI Status Badge](https://github.com/GoogleChrome/android-browser-helper/workflows/Android%20CI/badge.svg)

The Android Browser Helper library helps developers use Custom Tabs and Trusted
Web Activities on top of the AndroidX browser support library.
It contains default implementations of many of the common tasks a
developer will find themselves requiring, for example:

* Creating a Launcher Activity that simply launches a Trusted Web Activity.
* Code for choosing an appropriate Custom Tabs provider.
* Creating an Activity to launch the browser's site settings for a TWA.

## Adding Android Browser Helper to an Android project

Android Browser helper is available on the Google Maven. To use it, modify your application's
`build.gradle` and add the library as a dependency, as described below:

```gradle
dependencies {
    //...
    implementation 'com.google.androidbrowserhelper:androidbrowserhelper:0.1.0-alpha1'
}

``` 

**Important:** Since Android Browser Helper depends on a version of `androidx.browser` that is not
yet stable, the library is still marked as alpha. This will be updated once all the libraries
it depends on are stable.

**Warning:** Due to API changes on the latest Alpha version of `androidx.browser`, which Android
Browser Helper depends on, the current version of Android Browser Helper, `0.1.0-alpha1`, is not
compatible with versions of `androidx.browser` starting from `1.2.0-alpha09`. We are working
on an `alpha2` version of Android Browser Helper, that will fix the compatibility.
  
## Source Code Headers

Every file containing source code must include copyright and license
information. This includes any JS/CSS files that you might be serving out to
browsers. (This is to help well-intentioned people avoid accidental copying that
doesn't comply with the license.)

Apache header:

    Copyright 2019 Google LLC

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        https://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
