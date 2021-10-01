# BUTTONS IN ANDROID

<b>What is a button in android studio?</b>

In Android Studio, Button allows users to perform actions and make choices, when they are
clicked, tapped or pressed. Button represents a push button.
A button can consist of text or an icon or both text and an icon, which when clicked let us
know what actions are going to be performed. It is a very common widget in Android and
developers often use it.

Types of buttons in android studio are button, imagebutton, checkbox, switch, chip, radio
button etc

<p align="center" width="100%"><img src="/types.png"></p>

<p align="center" width="100%"><img src="images/button_in_android.png" width="500px"></p>

## <p>Xml Code of button</p>

```xml
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
<Button
    android:id="@+id/button"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Hello"
    app:layout_constraintBottom_toBottomOf="parent"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintHorizontal_bias="0.5"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toTopOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>
```

## <p>Xml Attributes</p>

Here are some important attributes to configure a Button in xml layout.\

<p><b>1. id </b>: id is an attribute which uniquely identifies a text Button.</p>
Below is the example code in which we set the id of a Button.

```xml
<Button
    android:id="@+id/button"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Hello World"
    android:textColor="#FFFFFF"
    app:backgroundTint="#673AB7"/>
```

<br>

<p><b>2. gravity </b>: The gravity attribute specifies the alignment of the text in the button like left,
right, center, top, bottom, center_vertical, center_horizontal, bottom_start etc.
Here we have used bottom_start gravity.</p>

```xml
<Button
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:id="@+id/button"
    android:gravity="bottom|start"
    android:text="Hello"
    android:textColor="#FFFFFF"
    app:backgroundTint="#673AB7"/>
```

<p align="center"><img src="images/pic2.png"></p>
<br>

<p><b>3. text </b>: text attribute displays the text of a Button.
We can display text in XML and Java class both.
</p>

```xml
<Button
    android:id="@+id/button"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text=" Android Development"
    android:textAllCaps="false"
    android:textColor="#FFFFFF"
    app:backgroundTint="#673AB7"/>
```

<br>
<p align="center"><img src="images/pic3.png"></p>
<br>

## Set Text Using Java Class:

<b>In the code below, we have set the text on Button in java class</b>

```xml
Button button = (Button) findViewById(R.id.button);
button.setText("Android Development");//set the text on button
```

<br>
<p><b>4. textColor </b>: textColor attribute displays the color of the text.
</p>

```xml
<Button
    android:id="@+id/button"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text=" Android Development"
    android:textAllCaps="false"
    android:textColor="#00BCD4"
    app:backgroundTint="#673AB7"/>
```

<br>
<p align="center"><img src="images/pic4.png"></p>
<br>

## Set Text Color On Button In Java class:

<b>In the code below, we have set the text color on Button in java class</b>

```xml
Button button=(Button) findViewById(R.id.button);
button.setTextColor(Color.BLUE);//set the blue color for the text
```

<br>
<p><b>5. textSize </b>: textSize attribute displays the size of the text on Button. We can display text
in sp (scale independent pixel) and dp (density independent pixel) units.

</p>

```xml
<Button
    android:id="@+id/button"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text=" Android Development"
    android:textAllCaps="false"
    android:textColor="#00BCD4"
    android:textSize="24sp"
    app:backgroundTint="#673AB7"/>
```

<br>
<p align="center"><img src="images/pic5.png"></p>
<br>
## Set textSize In Java class:

<p><b>In the code below, we have set the text size of buttons in java class.</b></p>

```xml
Button button=(Button)findViewById(R.id.button);
button.setTextSize(24);//set the text size of button
```

<br>
<p><b>6. textStyle </b>:  textStyle attribute displays the style of a text. Some text styles are bold, italic
and normal. To use more than one text style for a Button us â€œ|â€ operator.
</p>

```xml
<Button
    android:id="@+id/button"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text=" Android Development"
    android:textAllCaps="false"
    android:textColor="#00BCD4"
    android:textSize="24sp"
    android:textStyle="bold|italic"
    app:backgroundTint="#673AB7"/>
```

<br>
<p align="center"><img src="images/pic6.png"></p>
<br>

<p><b>7. background </b>: background attribute displays the background of a Button. We can
display a color or a drawable in the background of a Button.
</p>

```xml
<Button
    android:id="@+id/button"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text=" Android Development"
    android:textAllCaps="false"
    android:textColor="#00BCD4"
    android:textSize="24sp"
    android:textStyle="bold|italic"
    app:backgroundTint="#E91E63"/>
```

<br>
<p align="center"><img src="images/redappdevelopment.png"></p>
<br>

## Set background in Button In Java class:

<p><b>In the code below, we have set the background color of buttons in java class.</b></p>

```xml
Button button=(Button)findViewById(R.id.button);
button.setBackgroundColor(Color.PINK);//set the pink color of
button background
```

<br>
<p><b>8. padding </b>:  padding attribute is used to set the padding from left, right, top or bottom.
</p>
<p>In the below example code we have set paddings from all the sides.
</p>

```xml
<Button
    android:id="@+id/button"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:paddingLeft="24dp"
    android:paddingTop="14dp"
    android:paddingRight="24dp"
    android:paddingBottom="14dp"
    android:text=" Android Development"
    android:textAllCaps="false"
    android:textColor="#00BCD4"
    android:textSize="24sp"
    android:textStyle="bold|italic"
    app:backgroundTint="#E91E63"/>
```

<br>
<p align="center"><img src="images/redappdevelopment2.png"></p>
<br>

## Making buttons attractive

### Round button

<b>In XML Layout</b>

```xml
<Button
    android:id="@+id/button"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Hello"
    app:cornerRadius="20dp"
    app:layout_constraintBottom_toBottomOf="parent"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintHorizontal_bias="0.5"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toTopOf="parent"
    app:layout_constraintVertical_bias="0.499" />
```

<p align="center"><img src="images/pic2.png"></p>
<br>

## Gradient button

Making gradient colors is fun. Because they look just like magic when one color changes to another.

First make a drawable file. Name it gradientbutton.xml.
<br>

<p align="center"><img src="images/gradient.png" width="400px"></p>

<b>In drawable file:</b> \
 <br>
We need gradient, shape and corners. For gradient we have used two color values, startColor and endColor. Set the corner radius.

```xml
<?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/ndroid">
    <gradient
        android:startColor="@color/design_default_color_primary"
        android:endColor="@color/teal_200"
    />
    <corners
        android:radius="80dp"
    />
</shape>
```

<b>In XML Layout</b>

```xml
<Button
    android:id="@+id/button"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:onClick="openButton"
    android:paddingLeft="24dp"
    android:paddingTop="14dp"
    android:paddingRight="24dp"
    android:paddingBottom="14dp"
    android:text=" Android Development"
    android:textAllCaps="false"
    android:textColor="#ffffff"
    android:textSize="24sp"
    android:textStyle="bold|italic"
    app:backgroundTint="@drawable/gradientbutton"
    android:background="@drawable/gradientbutton"/>
```

<br>
<p align="center"><img src="images/gradient2.png" width="400px"></p>
<br>
<b>Outlined buttons:</b> 
 <br>
 Make a drawable file. Name it borderbutton.xml. <br>
 We need a selector, item, shape for this. <br>
 Set shape to rectangle, solid with color, stroke with width and color.
<br>
<br>
<p><b>In drawable file:</b></p>

```xml
<?xml version="1.0" encoding="utf-8"?>
    <selector xmlns:android="http://schemas.android.com/apk/res/android">
        <item>
            <shape xmlns:android="http://schemas.android.com/apk/res/android" android:shape="rectangle">
                <solid android:color="@color/purple_200"/>
                    <stroke android:width="5px" android:color="@color/black"/>
            </shape>
        </item>
    </selector>
```

<b>In XML Layout</b>

```xml
<Button
    android:id="@+id/button"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:onClick="openButton"
    android:paddingLeft="24dp"
    android:paddingTop="14dp"
    android:paddingRight="24dp"
    android:paddingBottom="14dp"
    android:text=" Android Development"
    android:textAllCaps="false"
    android:textColor="#ffffff"
    android:textSize="24dp"
    android:textStyle="bold|italic"
    app:backgroundTint="@drawable/gradientbutton"
    android:background="@drawable/borderbutton"
    app:cornerRadius="80dp"/>
```

<br>
<p align="center"><img src="images/pic.png" width="400px"></p>
<br>

## Contained button

Note The contained button is the default style in android studio

<p align="center"><img src="images/containedbutton.png" width="400px"></p>
<br>

In xml Layout

```xml
<Button
    android:id="@+id/button"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Contained Button"
    android:textColor="#FFFFFF"
    app:backgroundTint="#673AB7"
    app:layout_constraintBottom_toBottomOf="parent"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintHorizontal_bias="0.5"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toTopOf="parent" />
```

## Buttons with icon and text:

Lots of designs for buttons in Android use icons and text for buttons.<br>
To create these types of buttons we use some attributes. The attribute drawableBottom is the drawable to be drawn below the text. <br>
Similarly drawableRight for right of the text. <br>
Letâ€™s see how to add an icon to a button at the start of the text, at bottom, at end and at top
of the text. <br>
We have taken the default Android icon from the drawable resource manager
<br>

<p align="center"><img src="images/pic7.png"> </p>

<p><b>XML Code for icon below the text.</b></p>

```xml
<Button
    android:id="@+id/button"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:onClick="openButton"
    android:paddingLeft="24dp"
    android:paddingTop="14dp"
    android:paddingRight="24dp"
    android:paddingBottom="14dp"
    android:text=" Android Development"
    android:textAllCaps="false"
    android:textColor="#ffffff"
    android:textSize="24dp"
    android:textStyle="bold|italic"
    app:backgroundTint="@drawable/gradientbutton"
    android:background="@drawable/gradientbutton"
    android:drawableBottom="@drawable/ic_launcher_foreground"/>
```

<p align="center"><img src="images/pic8.png"> </p>
<br>
<p align="center"><img src="images/pic9.png"> </p>
<br>

### For icon at top of the text

```xml
android:drawableTop="@drawable/ic_launcher_foreground"
```

<p align="center"><img src="images/pic10.png"> </p>
<br>

### For icon at top of the text

```xml
android:drawableTop="@drawable/ic_launcher_foreground"
```

<p align="center"><img src="images/pic10.png"> </p>
<br>

### For icon at the start of text

```xml
android:drawableLeft="@drawable/ic_launcher_foreground"
```

<br>

## ANATOMY FOR OUTLINED BUTTON WITH TEXT AND ICON

It has a text label, a stroked container and an optional icon.

<p align="center"><img src="images/button.png"> </p>
<br>
   1. Text label<br>
   2. Container<br>
   3. icon <br>

## ANATOMY FOR CONTAINED BUTTON WITH TEXT AND ICON

<br>
<p align="center"><img src="images/button2.png"> </p>
<br>

## Circle button

To make a circle button, we need a new drawable. Name it circle.xml.<br>
We need a selector, item and shape. Use an oval for shape. Take the width and height size
the same to make the button circular. Set the size with the size tag. Also set color with solid
to any color code. Now you can use your drawable for the background attribute of your
button.<br>
<br>

<b>In xml Layout</b>

```xml
<Button
    android:id ="@+id/button"
    android:layout_width="150dp"
    android:layout_height="150dp"
    android:text="Round Button"
    android:background="@drawable/circle"
    android:padding="15dp"/>
```

<b>In drawable file</b>

```xml
<?xml version="1.0" encoding="utf-8"?>
<selector xmlns:android="http://schemas.android.com/apk/res/android">
    <item>
        <shape android:shape="oval">
            <stroke android:color="#1E90FF" android:width="5dp" />
                <solid android:color="#87CEEB"/>
                    <size android:width="150dp" android:height="150dp"/>
        </shape>
    </item>
</selector>
```

<p align="center"><img src="images/round.png"> </p>
<br>

# Responding to Click Events

When a user clicks a button, the button receives an on click event.<br>
We add the android:onClick attribute to the button element in XML layout. The value of the
attribute is the name of the method we call in response to a click event. Then the Activity
hosting the layout, implements the method.<br>
Here is an example for this:

<b>In xml layout setting onclick</b>
<br>

```xml
<Button
    android:id="@+id/button"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:onClick="openButton"
    android:paddingLeft="24dp"
    android:paddingTop="14dp"
    android:paddingRight="24dp"
    android:paddingBottom="14dp"
    android:text=" Android Development"
    android:textAllCaps="false"
    android:textColor="#00BCD4"
    android:textSize="24sp"
    android:textStyle="bold|italic"
    app:backgroundTint="#E91E63"
    app:layout_constraintBottom_toBottomOf="parent"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintHorizontal_bias="0.5"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toTopOf="parent" />
```

<p><b>In java code making a toast </b></p>

#### Here using the openButton() method on the button and using Toast we will display which button is clicked by the user.

```xml
public class MainActivity extends AppCompatActivity {
Button button;
@Override
protected void onCreate(Bundle savedInstanceState) {
super.onCreate(savedInstanceState);
setContentView(R.layout.activity_main);
button = findViewById(R.id.button); //get id of button
}
public void openButton(View v){
Toast.makeText(this, "Learn Android Development",
Toast.LENGTH_SHORT).show();
}
}
```

## Result:

#### Now start the AVD in Emulator and run the app. There is a button. Click on it and you will see a message on screen when the button is clicked.

<br>
<p align="center">![onclick event](https://user-images.githubusercontent.com/80222700/135617065-67db2511-df36-466a-8d7f-32a27b631680.png)</p>
<br>

## References:

<a>https://developer.android.com/reference/android/widget/Button</a><br>
<a>https://developer.android.com/guide/topics/ui/controls/button</a><br>
<a>https://material.io/components/buttons/android</a>
