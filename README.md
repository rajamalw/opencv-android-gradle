# opencv-android-gradle
OpenCV Android SDK modified to use in Android Studio

OpenCV SDK Version
-------
3.1.0
Download JAR
--------
[JAR][1]

Usage
--------
1.Copy the __opencv-android.jar__ to __app->libs__ in your project.

2.Open build.gradle and add the following line to the dependencies block.
```
compile files('libs/opencv-android.jar')
```
3.Sync the project.

To Build JAR in Linux
--------
1.Create a __local.properties__ file and define Android SDK path.

```
sdk.dir=/home/rajamalw/android-sdk-linux
```
Here __/home/rajamalw/android-sdk-linux__ is my SDK path. Replace with your SDK path.

2.Export Gradle path. For example in Ubuntu.
```shell
export PATH="/home/rajamalw/gradle/gradle-2.10/bin:$PATH"
```
where __/home/rajamalw/gradle/gradle-2.10/bin__ is the path where my Gradle executable is present.

3.Use the following Commands to generate JAR.
```
gradle build
gradle jar
```
4.The JAR will be generated in __build/libs__. 



[1]:https://github.com/rajamalw/opencv-android-gradle/raw/master/jar/opencv-android.jar
