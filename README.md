## Ex.No:1 Implementation of a Hello world Activity using all lifecycles methods using Android Studio.
## AIM:

To create Hello world Activity using all lifecycles methods to display messages using android studio.


## EQUIPMENTS REQUIRED:

Android Studio(Min. required Artic Fox)


## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.


## PROGRAM:
/*
Program to implement a Hello world Activity using all lifecycles methods using Android Studio                                                                      
Developed by: DHANALAKSHMI S                                                                        
RegisterNumber: 212222040033
*/

## MainActivity.java:
```
package com.example.experiment1;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.Toast;
public class MainActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast=Toast.makeText(getApplicationContext(),"OnCreate Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStart(){
        super.onStart();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStart Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onResume(){
        super.onResume();
        Toast toast=Toast.makeText(getApplicationContext(),"OnResume Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onPause(){
        super.onPause();
        Toast toast=Toast.makeText(getApplicationContext(),"OnPause Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStop(){
        super.onStop();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStop Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onRestart() {
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "OnRestart Executed", Toast.LENGTH_LONG);
        toast.show();

    }
    protected void onDestroy(){
        super.onDestroy();
        Toast toast=Toast.makeText(getApplicationContext(),"OnDestroy Executed",Toast.LENGTH_LONG);
        toast.show();
    }
}
```
## activitymain.xml:
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```


## OUTPUT:

## OnCreate Executed

![WhatsApp Image 2024-09-10 at 17 51 57_ed1b41f1](https://github.com/user-attachments/assets/3e8d80be-3fd6-42f8-b03c-889daa9f8f98)

## OnStop Executed 

![WhatsApp Image 2024-09-10 at 17 51 43_bc1a2648](https://github.com/user-attachments/assets/9b7d3a1c-9207-4f01-a083-12dc72867c8f)

## OnStart Executed

![WhatsApp Image 2024-09-10 at 18 27 04_53b779d2](https://github.com/user-attachments/assets/4a8a22fc-fd2d-4060-a025-96d1f819c79a)

## OnResume Executed

![WhatsApp Image 2024-09-10 at 18 22 30_c2c4e6eb](https://github.com/user-attachments/assets/a0b73711-ffce-496e-b96d-6b3c56f4a107)

## RESULT:
Thus a program to implement the various life cycles of an activity is written and successfully executed using Android Studio.
