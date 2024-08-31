# BASIC-ANDROID-_EX_01_Implementation of a Hello world Activity using all lifecycles methods using Android Studio.


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


## PROGRAM
### DEVELOPED BY : Mohamed Anas O.I
### REGISTER NO: 212223110028

### MainActivity.java:
```
package com.example.helloworld;

import android.os.Bundle;
import android.widget.Toast;

import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AppCompatActivity;
import androidx.core.graphics.Insets;
import androidx.core.view.ViewCompat;
import androidx.core.view.WindowInsetsCompat;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast t=Toast.makeText(this, "oncreat called", Toast.LENGTH_SHORT);
        t.show();

    }
    protected void onStart() {
        super.onStart();
        super.onResume();
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onStart called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onResume() {
        super.onResume();
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onResume called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onRestart() {
        super.onRestart();
        super.onResume();
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onRestart called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onPause() {
        super.onPause();
        super.onResume();
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onpasue called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStop() {
        super.onStop();
        super.onResume();
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onstop called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onDestroy() {
        super.onDestroy();
        super.onResume();
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "ondestroy called", Toast.LENGTH_LONG);
        toast.show();
    }
}
```
### Activity_Main.XML:
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView"
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

![WhatsApp Image 2024-08-30 at 18 36 53_2f94802a](https://github.com/user-attachments/assets/5d043f7b-f56b-48c4-b3a9-eb12b60fac92)

![WhatsApp Image 2024-08-30 at 18 36 54_1c1897e5](https://github.com/user-attachments/assets/ead36a00-1bfd-4de3-ad96-83089fd92923)

![WhatsApp Image 2024-08-30 at 18 36 54_7e133442](https://github.com/user-attachments/assets/c1307373-9882-428d-86f0-926e943d0aec)



## RESULT:
Thus a program to implement the various life cycles of an activity is written and successfully executed using Android Studio.

