# 📱Assignment 2 (Student Details Form App) 

## 📌 Overview

This is a simple Android application built using **Java** and **XML** that allows users to enter and submit student details such as **Name, City, Course, and Email**.

The app demonstrates:

* UI design using XML
* Toolbar integration
* User input handling
* Toast message display

This project is perfect for beginners learning Android development.

---

## 🚀 Features

* 📋 User-friendly Student Form UI
* 🧾 Input fields:

  * Name
  * City
  * Course
  * Email
* 🔘 Submit button to display entered data
* 🧭 Toolbar with title & subtitle
* 📱 Edge-to-edge layout support
* ⚡ Simple and lightweight app

---

## 🛠️ Tech Stack

* **Language:** Java
* **UI:** XML (Android Layouts)
* **Framework:** Android SDK
* **IDE:** Android Studio

---

## 📂 Project Structure

```
app/
 ├── java/com/example/assignment2/
 │    └── MainActivity.java
 │
 ├── res/
 │    ├── layout/
 │    │    └── activity_main.xml
 │    │
 │    ├── values/
 │    │    ├── colors.xml
 │    │    ├── strings.xml
 │    │    └── themes.xml
 │
 └── AndroidManifest.xml
```

---

## 🧩 Layout (XML)

The UI is designed using a **LinearLayout** structure with:

* Toolbar (AppBar)
* Title TextView ("Student Details")
* Multiple input fields using EditText
* Submit Button

### 🔹 Key Components:

* `EditText` → for user input
* `TextView` → labels
* `Button` → submit action
* `Toolbar` → app header

---

## ⚙️ MainActivity (Java Logic)

### 🔹 Key Functionalities:

* Initialize UI components using `findViewById`
* Setup Toolbar with:

  * Title → *Student Details*
  * Subtitle → *Welcome to the Form*
* Handle button click event
* Capture user input
* Display output using **Toast**

### 🔹 Core Logic:

```java
String name = nameET.getText().toString();
String city = cityEt.getText().toString();
String course = courseET.getText().toString();
String email = emailET.getText().toString();

String output = "My name is " + name +
                " I live in " + city +
                " and my course and email id is: " +
                course + " " + email;

Toast.makeText(getApplicationContext(), output, Toast.LENGTH_SHORT).show();
```

---

## 📸 Screenshot

👉 *(Add your app screenshot here)*

Example:

```
![App Screenshot](screenshots/app.png)
```

---

## ▶️ How to Run

1. Clone the repository:

```
git clone https://github.com/your-username/student-details-app.git
```

2. Open the project in **Android Studio**

3. Sync Gradle

4. Run the app on:

   * Android Emulator OR
   * Physical Device

---

## 🧪 How It Works

1. User enters details in the form
2. Clicks on **Submit**
3. App collects data from EditText fields
4. Displays a formatted message using Toast

---

## 🔮 Future Improvements

* ✅ Add input validation (empty fields, email format)
* 🎨 Upgrade UI using Material Design (TextInputLayout)
* 💾 Store data using SQLite or Firebase
* 📄 Add multiple activities/screens
* 🔔 Replace Toast with AlertDialog

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a new branch
3. Commit your changes
4. Submit a Pull Request

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 🙌 Author

**Divyansh Jain**
GitHub: https://github.com/Divyansh-jain2005

---

# 📱Assignment 3 (Basic Calculator App)

A simple and user-friendly **Basic Calculator Android App** built using **Java** and **XML**. This app performs basic arithmetic operations like Addition, Subtraction, Multiplication, and Division.

---

## 🚀 Features

* ➕ Addition
* ➖ Subtraction
* ✖️ Multiplication
* ➗ Division
* 📥 User input validation
* ⚠️ Handles divide-by-zero errors
* 🎨 Clean and responsive UI

---

## 🛠️ Tech Stack

* **Language:** Java
* **UI Design:** XML
* **IDE:** Android Studio
* **Minimum SDK:** (Add your version here)

---

## 📂 Project Structure

```
📦 BasicCalculator
 ┣ 📂 java/com/example/assignment3
 ┃ ┗ 📜 MainActivity.java
 ┣ 📂 res/layout
 ┃ ┗ 📜 activity_main.xml
 ┣ 📂 res/values
 ┃ ┗ 📜 colors.xml
 ┗ 📜 AndroidManifest.xml
```

---

## 📸 Screenshots

> Add your app screenshots here
> Example:

```
![App Screenshot](screenshots/calculator.png)
```

---

## 💡 How It Works

1. User enters two numbers
2. Clicks any operation button (+, −, ×, ÷)
3. Result is displayed instantly

---

## 🔢 Core Logic (Java)

```java
add.setOnClickListener(v -> {
    double a = Double.parseDouble(num1.getText().toString());
    double b = Double.parseDouble(num2.getText().toString());
    addEt1.setText(String.valueOf(a + b));
});
```

✔ Similar logic is used for Subtraction, Multiplication, and Division
✔ Division includes zero-check to prevent errors

---

## 🎨 UI Layout (XML)

* Uses **LinearLayout** for structure
* Input fields for numbers
* Buttons for operations
* TextViews to display results

```xml
<Button
    android:id="@+id/add"
    android:text="+"
    android:layout_width="0dp"
    android:layout_weight="1"
    android:layout_height="wrap_content"/>
```

---

## ⚠️ Error Handling

* Prevents app crash on empty input
* Handles divide-by-zero case
* Ensures smooth user experience

---

## 📌 Future Improvements

* 🧮 Add scientific calculator features
* 🌙 Dark mode support
* 🎯 Better UI with Material Design
* 🔄 Add clear/reset button

---

## 🧑‍💻 Author

**Divyansh Jain**
GitHub: https://github.com/Divyansh-jain2005

---

## 📄 License

This project is open-source and available under the MIT License.

---


# 📱Assignment 4 (User Preference Application) 

## 📌 Project Overview

This is a simple **Android application** developed using **Java and XML** that collects user information such as name, mobile number, address, gender, date of birth, and hobbies. After submission, the app displays all the entered details in a structured format.

---

## 🚀 Features

* 🧑 User Input Form (Name, Mobile, Address)
* 🚻 Gender Selection using Radio Buttons
* 📅 Date Picker Dialog for selecting Date of Birth
* 🎯 Hobby Selection using CheckBoxes
* 📄 Display of user details on button click
* ⚠️ Basic validation (e.g., gender selection)

---

## 🛠️ Technologies Used

* **Java** (Backend logic)
* **XML** (UI Design)
* **Android Studio**
* **Android SDK Components**

  * `EditText`
  * `RadioGroup`
  * `CheckBox`
  * `DatePickerDialog`
  * `TextView`
  * `Button`

---

## 📂 Project Structure

```
com.example.assignment4
│
├── MainActivity.java
└── res
    └── layout
        └── activity_main.xml
```

---

## 📱 UI Components

### 🧾 Input Fields

* Name
* Mobile Number
* Address

### 🚻 Gender Selection

* Male
* Female
* Other

### 📅 Date of Birth

* Selected using a DatePicker dialog

### 🎯 Hobbies

* Reading Books
* Dancing
* Singing
* Travelling

---

## ⚙️ How It Works

1. User enters personal details.
2. Selects gender using RadioButtons.
3. Clicks **"Select Date"** to pick DOB.
4. Chooses hobbies via CheckBoxes.
5. Clicks **SUBMIT** button.
6. App displays formatted output in TextView.

---

## 🧠 Core Logic

### 📅 Date Picker Implementation

* Uses `DatePickerDialog`
* Displays selected date on button

### 📊 Form Submission

* Collects all inputs
* Validates gender selection
* Builds output string using `StringBuilder`
* Displays result in TextView

---

## 🧾 Sample Output

```
My name is Divyansh
Mobile: 9876543210
DOB: 12/04/2004
Gender: Male
Hobbies: Reading Books, Dancing
```

---

## ⚠️ Validations Implemented

* Gender must be selected
* Prevents app crash if no selection is made

---

## 🎨 UI Highlights

* Simple and clean layout using LinearLayout
* Organized sections for better readability
* Responsive padding and spacing

---

## 📸 Screenshots

*(Add your app screenshots here)*

### Home Screen

![Home Screen](screenshots/home.png)

### Output Screen

![Output Screen](screenshots/output.png)

---

## 🔧 Future Improvements

* Add input validation (empty fields, mobile format)
* Use **ConstraintLayout** for better performance
* Upgrade UI using **Material Design**
* Store user data using SQLite or Firebase
* Add dark mode 🌙

---

## ▶️ How to Run

1. Open project in **Android Studio**
2. Connect emulator or Android device
3. Click **Run ▶️**
4. Test the application

---


## 🧑‍💻 Author

**Divyansh Jain**
GitHub: https://github.com/Divyansh-jain2005

---

## 📜 License

This project is for educational purposes.

---
# 📅Assignment 5 (Android Date Picker App)

A simple Android application built using **Java** that allows users to select a date using a **DatePicker** and display the selected date on the screen.

---

## 🚀 Features

* 📆 Select date using DatePicker
* 🔘 Submit button to confirm selection
* 📝 Displays selected date in TextView
* 📱 Clean and simple UI design
* ⚡ Uses modern Edge-to-Edge layout support

---

## 🛠️ Technologies Used

* Java
* Android SDK
* XML (UI Design)
* Android Studio

---

## 📂 Project Structure

```
Assignment5/
│── java/com/example/assignment5/
│     └── MainActivity.java
│
│── res/layout/
│     └── activity_main.xml
```

---

## 📄 XML Layout (activity_main.xml)

```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:gravity="center"
    tools:context=".MainActivity">

    <DatePicker
        android:id="@+id/datepicker"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content" />

    <Button
        android:id="@+id/btn"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="SUBMIT"
        android:layout_marginTop="20dp"/>

    <TextView
        android:id="@+id/output"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Selected Date:"
        android:textSize="20sp"
        android:layout_marginTop="20dp"/>

</LinearLayout>
```

---

## 💻 Java Code (MainActivity.java)

```java
package com.example.assignment5;

import android.os.Bundle;
import android.widget.Button;
import android.widget.DatePicker;
import android.widget.TextView;

import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AppCompatActivity;
import androidx.core.graphics.Insets;
import androidx.core.view.ViewCompat;
import androidx.core.view.WindowInsetsCompat;

public class MainActivity extends AppCompatActivity {

    Button btn;
    DatePicker dp;
    TextView output;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        EdgeToEdge.enable(this);
        setContentView(R.layout.activity_main);

        // Handle edge-to-edge padding
        ViewCompat.setOnApplyWindowInsetsListener(findViewById(R.id.main), (v, insets) -> {
            Insets systemBars = insets.getInsets(WindowInsetsCompat.Type.systemBars());
            v.setPadding(systemBars.left, systemBars.top, systemBars.right, systemBars.bottom);
            return insets;
        });

        // Initialize views
        btn = findViewById(R.id.btn);
        dp = findViewById(R.id.datepicker);
        output = findViewById(R.id.output);

        // Button click event
        btn.setOnClickListener(v -> {
            int day = dp.getDayOfMonth();
            int month = dp.getMonth() + 1;
            int year = dp.getYear();

            output.setText("Selected Date: " + day + "/" + month + "/" + year);
        });
    }
}
```

---

## 📸 Screenshot

*Add your app screenshot here*

```
![App Screenshot](screenshot.png)
```

---

## ⚙️ How to Run

1. Open the project in **Android Studio**
2. Connect an emulator or physical device
3. Click ▶️ Run
4. Select a date and press **SUBMIT**

---

## 📌 Future Improvements

* 🎨 Improve UI using Material Design
* 📅 Add DatePicker Dialog
* 🌍 Add date format options
* 🔔 Show Toast message on selection

---

## 👨‍💻 Author

**Divyansh Jain**
GitHub: https://github.com/Divyansh-jain2005

---

## 📜 License

This project is for educational purposes.



This project is for educational purposes.
