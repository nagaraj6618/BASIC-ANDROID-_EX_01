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

Program to implement a Hello world Activity using all lifecycles methods using Android Studio                                                                      
Developed by: NAGARAJ S                                                                        
RegisterNumber: 212221040109


## MainActivity.java:
```
package com.example.experiment_1;

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

![oncreate](https://github.com/user-attachments/assets/7b3258a7-32a3-482b-9db2-e7e3c7b1108b)


## OnStart Executed 

![onstart)](https://github.com/user-attachments/assets/291af358-907a-44bd-ae68-620d95abb325)


## OnResume Executed

![onresume](https://github.com/user-attachments/assets/2400d0c9-004e-4683-9e2c-25e94e3f8a20)

## OnRestart Executed

![onrestart](https://github.com/user-attachments/assets/ea7d0996-b4ad-40bf-a3f2-529d98162ce0)


## onPause Executed

![onpause)](https://github.com/user-attachments/assets/6eb5a263-1bb5-4162-a7d5-aa69fce79bbe)



## RESULT:
Thus a program to implement the various life cycles of an activity is written and successfully executed using Android Studio.
