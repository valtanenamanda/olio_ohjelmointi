package org.viikko8.myapplication;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.view.View;
import android.widget.EditText;
import android.widget.TextView;

public class MainActivity extends AppCompatActivity {

    private EditText textInput1;

    private EditText textInput2;

    private TextView textOutput;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        textInput1 = findViewById(R.id.editText);
        textInput2 = findViewById(R.id.editText2);
        textOutput = findViewById(R.id.textView);
    }

    public void add(View view) {
        int number1 = Integer.parseInt(textInput1.getText().toString());
        int number2 = Integer.parseInt(textInput2.getText().toString());
        int sum = number1 + number2;
        String x = Integer.toString(sum);
        textOutput.setText(x);
    }

    public void subtract(View view) {
        int number1 = Integer.parseInt(textInput1.getText().toString());
        int number2 = Integer.parseInt(textInput2.getText().toString());
        int sub = number1 - number2;
        String x = Integer.toString(sub);
        textOutput.setText(x);
    }

    public void multiply(View view) {
        int number1 = Integer.parseInt(textInput1.getText().toString());
        int number2 = Integer.parseInt(textInput2.getText().toString());
        int multiply = number1 * number2;
        String x = Integer.toString(multiply);
        textOutput.setText(x);
    }

    public void divide(View view) {
        int number1 = Integer.parseInt(textInput1.getText().toString());
        int number2 = Integer.parseInt(textInput2.getText().toString());
        int divide = number1 / number2;
        String x = Integer.toString(divide);
        textOutput.setText(x);
    }
}
