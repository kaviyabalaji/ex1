# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.
## AIM:
To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:
Latest Version Android Studio

## ALGORITHM:
Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
~~~
/*
Program to print the text “Hello World”.
Developed by: B.Kaviya
Registeration Number : 212221040079
*/
MainActivity.java:
  package com.example.helloworld;
  import androidx.appcompat.app.AppCompatActivity;
  import android.os.Bundle;
  import android.util.Log;
  import android.widget.Toast;

 public class MainActivity extends AppCompatActivity {

  private static final String TAG = "HelloWorldActivity";

@Override
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);
    Log.d(TAG, "onCreate: ");
    Toast.makeText(this, "onCreate", Toast.LENGTH_SHORT).show();
}

@Override
protected void onStart() {
    super.onStart();
    Log.d(TAG, "onStart: ");
    Toast.makeText(this, "onStart", Toast.LENGTH_SHORT).show();
}

@Override
protected void onResume() {
    super.onResume();
    Log.d(TAG, "onResume: ");
    Toast.makeText(this, "onResume", Toast.LENGTH_SHORT).show();
}

@Override
protected void onPause() {
    super.onPause();
    Log.d(TAG, "onPause: ");
    Toast.makeText(this, "onPause", Toast.LENGTH_SHORT).show();
}

@Override
protected void onStop() {
    super.onStop();
    Log.d(TAG, "onStop: ");
    Toast.makeText(this, "onStop", Toast.LENGTH_SHORT).show();
}

@Override
protected void onDestroy() {
    super.onDestroy();
    Log.d(TAG, "onDestroy: ");
    Toast.makeText(this, "onDestroy", Toast.LENGTH_SHORT).show();
}

@Override
protected void onRestart() {
    super.onRestart();
    Log.d(TAG, "onRestart: ");
    Toast.makeText(this, "onRestart", Toast.LENGTH_SHORT).show();
}
}
Activity_main.xml:
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout        xmlns:android="http://schemas.android.com/apk/res/android"
xmlns:app="http://schemas.android.com/apk/res-auto"
xmlns:tools="http://schemas.android.com/tools"
android:layout_width="match_parent"
android:layout_height="match_parent"
tools:context=".MainActivity">

<TextView
    android:layout_width="238dp"
    android:layout_height="105dp"
    android:text="Hello World!"
    android:textSize="100px"
    android:textStyle="italic"
    app:layout_constraintBottom_toBottomOf="parent"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintHorizontal_bias="0.591"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toTopOf="parent"
    app:layout_constraintVertical_bias="0.499" />

</androidx.constraintlayout.widget.ConstraintLayout>
~~~
# OUTPUT:
## onCreate()
![image](https://github.com/Anuayshh/HelloWorld/assets/127651217/dcb585f7-e16b-4737-b84c-f0208d48192f)


## onRestart()
![image](https://github.com/Anuayshh/HelloWorld/assets/127651217/93674089-17d2-4f5c-8303-85b62aebaac1)


## onPause()
![image](https://github.com/Anuayshh/HelloWorld/assets/127651217/6630b25c-0b00-45b1-a291-8c165a330e3d)


## onResume()
![image](https://github.com/Anuayshh/HelloWorld/assets/127651217/815b9669-9136-49de-8507-68f4bbce2392)


## onDestroy()
![image](https://github.com/Anuayshh/HelloWorld/assets/127651217/6c25367c-2e96-4bdb-b181-17717ff7974d)


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
