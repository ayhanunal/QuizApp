[![API](https://img.shields.io/badge/API-16%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=16)
[![Android-Studio](https://img.shields.io/badge/Android%20Studio-4.2+-orange.svg?style=flat)](https://developer.android.com/studio/)
![Language](https://img.shields.io/badge/language-Kotlin-orange.svg)

<h1 align="center"> Quizz App </h1>

<p align="center">
Quiz app consisting of countries and their flags. Find the correct answer among the 4 answers and proceed to the next question. If you give a wrong answer, the background of the button containing your answer will be red, if the correct answer it will be green. At the end of the application, you will see your score.
</p>


### Manifest
Set the screen orientation to portrait in the `manifest.xml` file. Also set theme and softInputMode for `MainActivity.kt`
```xml
<activity
    android:name=".ResultActivity"
    android:screenOrientation="portrait"></activity>
<activity
    android:name=".QuizQuestionsActivity"
    android:screenOrientation="portrait" />
<activity
    android:name=".MainActivity"
    android:screenOrientation="portrait"
    android:theme="@style/NoActionBarTheme"
    android:windowSoftInputMode="adjustResize">
```

## Usage

<p align="center">
when you first enter the app, type a name to get started
</p>

<p align="center">
  <img src='https://github.com/ayhanunal/QuizApp/blob/main/ss/1.png' width=300 heihgt=300> 
</p>

<p align="center">
Choose an answer for the next question and press the "Submit" button. If the answer is correct, you will receive a green notification. Go to the last question with the "Go to next Question" button.

</p>

<p align="center">
  <img src='https://github.com/ayhanunal/QuizApp/blob/main/ss/2.png' width=300 heihgt=300> 
  <img src='https://github.com/ayhanunal/QuizApp/blob/main/ss/3.png' width=300 heihgt=300> 
  <img src='https://github.com/ayhanunal/QuizApp/blob/main/ss/4.png' width=300 heihgt=300> 
</p>

Add background file for correct answer and wrong answer in drawable folder.

`wrong_option_border_bg.xml`
```xml
<?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android"
    android:shape="rectangle">

    <solid android:color="@android:color/holo_red_light" />

    <corners android:radius="5dp" />
</shape>
```

`correct_option_border_bg.xml`
```xml
<?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android"
    android:shape="rectangle">

    <solid android:color="@android:color/holo_green_light" />

    <corners android:radius="5dp" />
</shape>
```
<p align="center">
When the quiz is over, the score information will appear.
</p>

<p align="center">
  <img src='https://github.com/ayhanunal/QuizApp/blob/main/ss/5.png' width=300 heihgt=300> 
</p>















