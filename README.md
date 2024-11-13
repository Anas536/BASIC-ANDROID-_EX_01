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
![Screenshot 2024-11-13 084629](https://github.com/user-attachments/assets/eb0e7cd8-a5b8-4788-aa9b-b6d471e446fa)

![Screenshot 2024-11-13 084636](https://github.com/user-attachments/assets/5e46afef-1683-465c-a7d8-a7ffaf084e81)

![Screenshot 2024-11-13 084644](https://github.com/user-attachments/assets/92c2ee6e-1f24-477c-b108-d4941beb5748)

![Screenshot 2024-11-13 084652](https://github.com/user-attachments/assets/2dd5bb15-5b41-4b71-aae6-4f1c7b13b73a)

![Screenshot 2024-11-13 084658](https://github.com/user-attachments/assets/253e0f29-5d00-4040-80b9-b1889abad1ae)

## RESULT:
Thus a program to implement the various life cycles of an activity is written and successfully executed using Android Studio.

