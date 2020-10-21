# Java Script for beginners in AndroidStudio. 
package com.example.demo2;

import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

     @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);



        Button clickMe = findViewById(R.id.myButton);
        clickMe.setOnClickListener(new View.OnClickListener() {
            TextView txtView = findViewById(R.id.myText);
            @Override
            public void onClick(View v) {

                txtView.setText("Welcome To My App");
                 Toast.makeText(MainActivity.this, "Welcome ", Toast.LENGTH_SHORT).show();





            }

        });


    }
}
