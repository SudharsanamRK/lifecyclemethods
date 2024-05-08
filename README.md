# Ex.No:2 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED

Latest Version Android Studio

## ALGORITHM

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM
```
Program to print the text “Hello World”.
Developed by: Sudharsanam R K
Registeration Number : 212222040163
```
# In activity_main.xml
```xml
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools">

    <application
        android:allowBackup="true"
        android:dataExtractionRules="@xml/data_extraction_rules"
        android:fullBackupContent="@xml/backup_rules"
        android:icon="@mipmap/ic_launcher"
        android:label="@string/app_name"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/Theme.Bombastic"
        tools:targetApi="31">
        <activity
            android:name=".MainActivity"
            android:exported="true">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>

</manifest>
```
# In MainActivity.java
```java
package com.example.bombastic;

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
        Toast toast = Toast.makeText(getApplicationContext(), "onStart Called", Toast.LENGTH_LONG);
        toast.show();
    }

    @Override
    protected void onRestart() {
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onPause() {
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onResume() {
        super.onResume();
        Toast toast = Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop() {
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy() {
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        toast.show();
    }
}
```

## OUTPUT
![ACTIVITY_MAIN.XML](https://github.com/SudharsanamRK/lifecyclemethods/assets/115523484/4746ea84-88ec-4d76-af32-ba3946262f59)
![MAINACTIVITY.JAVA](https://github.com/SudharsanamRK/lifecyclemethods/assets/115523484/5e7fe4c1-2122-413d-94e9-27ec41804ebc)
![onCreate](https://github.com/SudharsanamRK/lifecyclemethods/assets/115523484/46ff9aea-6885-4f14-aab3-78152873f38c)
![onStart](https://github.com/SudharsanamRK/lifecyclemethods/assets/115523484/9d488f35-4621-433a-9505-658b766aadfa)
![onRestart](https://github.com/SudharsanamRK/lifecyclemethods/assets/115523484/88116b14-6631-4f06-9ddb-e63a7cf9dc2f)
![onResume](https://github.com/SudharsanamRK/lifecyclemethods/assets/115523484/60d3436a-196d-49d4-825c-d495e5ed4777)
![onPause](https://github.com/SudharsanamRK/lifecyclemethods/assets/115523484/c24557d9-f486-45e9-bdea-e214fac4011d)
![onStop](https://github.com/SudharsanamRK/lifecyclemethods/assets/115523484/8b8d6ba2-1455-4cd6-9820-62754ccbd214)
![onDestroy](https://github.com/SudharsanamRK/lifecyclemethods/assets/115523484/4564e676-2c28-4b31-af2a-50b22dfe789b)

## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
