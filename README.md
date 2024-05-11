# Ex.No:2 To create a HelloWorld Activity using all lifecycles methods to display messages.
## AIM:
To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.
## EQUIPMENTS REQUIRED:
Latest Version Android Studio
## ALGORITHM:
```
Step 1: Open Android Stdio and then click on File -> New -> New project.
Step 2: Then type the Application name as HelloWorld and click Next. 
Step 3: Then select the Minimum SDK as shown below and click Next.
Step 4: Then select the Empty Activity and click Next. Finally click Finish.
Step 5: Design layout in activity_main.xml.
Step 6: Display message give in MainActivity file.
Step 7: Save and run the application.
```
## PROGRAM:
## activity_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:textAlignment="viewEnd"
    android:textDirection="anyRtl"
    tools:context=".MainActivity">
    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        android:textSize="24sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>
```
## MainActivity.java
```
package com.example.myapplication;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.Toast;
public class MainActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStart() {
        super.onStart();
        Toast toast1 = Toast.makeText(getApplicationContext(), "onStart Called", Toast.LENGTH_LONG);
        toast1.show();
    }
    @Override
    protected void onRestart() {
        super.onRestart();
        Toast toast2 = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
        toast2.show();
    }
    protected void onPause() {
        super.onPause();
        Toast toast3 = Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG);
        toast3.show();
    }
    protected void onResume() {
        super.onResume();
        Toast toast4 = Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG);
        toast4.show();
    }
    protected void onStop() {
        super.onStop();
        Toast toast5 = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        toast5.show();
    }
    protected void onDestroy() {
        super.onDestroy();
        Toast toast6 = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        toast6.show();
    }
}
```
## OUTPUT
![1 (1)](https://github.com/Jayalakshm1/lifecyclemethods/assets/130430542/74a7a7ef-8870-4841-8228-372bd9188f0e)
![1 (2)](https://github.com/Jayalakshm1/lifecyclemethods/assets/130430542/0f4cf2d3-9fb5-4d4c-9f86-7a7bf8998fef)
![1 (3)](https://github.com/Jayalakshm1/lifecyclemethods/assets/130430542/3eea3c45-4ddf-4449-a35c-df15615162ac)
![1 (4)](https://github.com/Jayalakshm1/lifecyclemethods/assets/130430542/33465d0a-ae1f-4b94-9091-2321c92613c2)
![1 (5)](https://github.com/Jayalakshm1/lifecyclemethods/assets/130430542/77c8c22f-21c4-469c-9071-6f6627fa3770)
![1 (6)](https://github.com/Jayalakshm1/lifecyclemethods/assets/130430542/96b4ca9e-8dda-4be5-955a-87d95e3b5300)
## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
