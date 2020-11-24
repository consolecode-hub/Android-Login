# Login
Login Details

![Login Design Capture](https://user-images.githubusercontent.com/3745464/100104063-b4961a80-2e8b-11eb-936a-ecb671082420.PNG)

Try material login xml design

Android Login Screen
 

XML layout design for android

Android Material login screen with androidx dependency

buildToolsVersion 30.0.1

minSdkVersion 14

implementation 'com.google.android.material:material:1.0.0'

`
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@color/colorPrimary"
    tools:context=".MainActivity">
    <ImageView
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:scaleType="fitEnd"
        app:srcCompat="@drawable/bg_wave"/>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:orientation="vertical">
        <ScrollView
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_centerVertical="true"
            android:orientation="vertical"
            android:gravity="center">
            <LinearLayout
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_centerVertical="true"
                android:gravity="center"
                android:layout_centerHorizontal="true"
                android:orientation="vertical">
                <LinearLayout
                    android:layout_width="match_parent"
                    android:orientation="vertical"
                    android:gravity="center"
                    android:layout_height="match_parent">
                    <RelativeLayout
                        android:id="@+id/relativeLayout"
                        android:layout_width="match_parent"
                        android:layout_height="200dp"
                        android:background="@color/bg">
                        <LinearLayout
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:transitionName="tran"
                            android:layout_centerHorizontal="true"
                            android:layout_centerVertical="true"
                            android:gravity="center"
                            android:orientation="vertical">
                            <LinearLayout
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:orientation="horizontal">
                                <ImageView
                                    android:layout_width="100dp"
                                    android:layout_height="100dp"
                                    android:id="@+id/imageView"
                                    app:srcCompat="@drawable/ic_launcher" />
                            </LinearLayout>
                            <TextView
                                android:id="@+id/txt"
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:text="Console Login"
                                android:textColor="@color/colorPrimary"
                                android:textSize="25sp"
                                android:layout_marginTop="10dp"
                                android:textStyle="bold" />
                        </LinearLayout>
                    </RelativeLayout>
                    <TextView
                        android:layout_width="match_parent"
                        android:layout_height="5dp"
                        android:layout_below="@id/relativeLayout"
                        android:background="@color/colorPrimaryDark"
                        />
                    <TextView
                        android:id="@+id/textView"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:layout_below="@id/relativeLayout"
                        android:layout_centerHorizontal="true"
                        android:layout_marginTop="30dp"
                        android:gravity="center"
                        android:textColorHint="@color/white"
                        android:textColor="@color/white"
                        android:text="User Registration"
                        android:textAppearance="@style/Base.TextAppearance.AppCompat.Medium"
                        />
                    <LinearLayout
                        android:id="@+id/linearLayout"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_below="@id/textView"
                        android:orientation="vertical"
                        android:layout_margin="10dp"
                        android:padding="15dp">

                        <com.google.android.material.textfield.TextInputLayout
                            style="@style/Widget.MaterialComponents.TextInputLayout.OutlinedBox"
                            android:layout_width="match_parent"
                            android:textColorHint="@color/white"
                            android:textColor="@color/white"
                            app:boxStrokeColor="@color/white"
                            android:layout_height="wrap_content">

                            <com.google.android.material.textfield.TextInputEditText
                                android:id="@+id/editTextName"
                                android:layout_width="match_parent"
                                android:layout_height="wrap_content"
                                android:inputType="text"
                                android:textColorHint="@color/white"
                                android:textColor="@color/white"
                                app:backgroundTint="@color/white"
                                android:hint="Username" />
                        </com.google.android.material.textfield.TextInputLayout>

                        <com.google.android.material.textfield.TextInputLayout
                            style="@style/Widget.MaterialComponents.TextInputLayout.OutlinedBox"
                            android:layout_width="match_parent" android:textColorHint="@color/white"
                            android:textColor="@color/white"
                            android:layout_height="wrap_content">

                            <com.google.android.material.textfield.TextInputEditText
                                android:id="@+id/editTextEmail"
                                android:layout_width="match_parent"
                                android:layout_height="wrap_content"
                                android:inputType="textWebEmailAddress"
                                android:hint="Password" />
                        </com.google.android.material.textfield.TextInputLayout>
                    </LinearLayout>
                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:gravity="right"
                        android:layout_margin="10dp"
                        android:padding="15dp"
                        android:orientation="horizontal">
                        <Button
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            style="@style/Widget.AppCompat.Light.ActionButton.CloseMode"
                            android:text="Cancel"
                            android:textColor="@color/white"
                            app:backgroundTint="@color/white"
                            android:textAllCaps="false" />
                        <com.google.android.material.button.MaterialButton
                            android:layout_width="150dp"
                            android:layout_height="wrap_content"
                            app:cornerRadius="18dp"
                            android:elevation="5dp"
                            app:backgroundTint="@color/white"
                            android:textColor="@color/colorPrimary"
                            style="@style/AppTheme.RoundedCornerMaterialButton"
                            android:text="Login">
                        </com.google.android.material.button.MaterialButton>
                    </LinearLayout>
                </LinearLayout>
            </LinearLayout>
        </ScrollView>
    </LinearLayout>
</RelativeLayout>
`
