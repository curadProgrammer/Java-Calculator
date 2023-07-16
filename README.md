<h1>Calculator App</h1>

<h2>Overview</h2>
<p>The Calculator App is a Java application that provides a graphical user interface (GUI) for performing basic arithmetic calculations. It uses Swing components for the GUI and includes features such as number input, arithmetic operations, and result display.</p>
<p>Checkout the full tutorial <a href="https://www.youtube.com/watch?v=IuGh1pXLfhc">here</a></p>
<h2>Files</h2>

<ol>
  <li><strong>CalculatorApp.java</strong>: This file contains the main class <code>CalculatorApp</code>, which serves as the entry point for the application. It creates an instance of the <code>CalculatorGui</code> class and makes the GUI visible.</li>

  <li><strong>CalculatorGui.java</strong>: This file contains the <code>CalculatorGui</code> class, which extends <code>JFrame</code> and represents the main GUI window of the application. It sets up the GUI components, including a display field for showing the numbers and results, and buttons for number input and arithmetic operations. It also handles button click events to perform the calculations.</li>

  <li><strong>CalculatorService.java</strong>: This file contains the <code>CalculatorService</code> class, which provides the actual arithmetic calculations for the application. It includes methods for addition, subtraction, multiplication, and division.</li>

  <li><strong>CommonConstants.java</strong>: This file contains the <code>CommonConstants</code> class, which defines common constants used in the application, such as the application name, the size of the GUI window, and the configurations for the display field and buttons.</li>
</ol>

<h2>Usage</h2>

<p>To use the Calculator App, follow these steps:</p>

<ol>
  <li>Compile the Java files:</li>
  <pre><code>javac CalculatorApp.java CalculatorGui.java CalculatorService.java CommonConstants.java</code></pre>

  <li>Run the compiled Java program:</li>
  <pre><code>java CalculatorApp</code></pre>

  <li>The Calculator App GUI window will appear. You can enter numbers and perform arithmetic operations using the buttons.</li>

  <li>To enter numbers, click the respective number buttons (0-9).</li>

  <li>To perform arithmetic operations, click the corresponding operator buttons (+, -, x, /). The current number in the display field will be used as the first operand.</li>

  <li>To calculate the result, click the "=" button. The result will be displayed in the display field.</li>
</ol>

<h2>Class Details</h2>

<h3>1. CalculatorApp.java</h3>

<p>This class contains the <code>CalculatorApp</code> class, which serves as the entry point for the application.</p>

<h4>Methods</h4>
<ul>
  <li><code>main(String[] args)</code>: The main method creates an instance of <code>CalculatorGui</code> and makes the GUI visible.</li>
</ul>

<h3>2. CalculatorGui.java</h3>

<p>This class represents the main GUI window of the application.</p>

<h4>Constructors</h4>
<ul>
  <li><code>CalculatorGui()</code>: Constructs a new <code>CalculatorGui</code> object. It sets up the JFrame with the application name, size, and close operation. It then calls the <code>addGuiComponents()</code> method to add the GUI components.</li>
</ul>

<h4>Methods</h4>
<ul>
  <li><code>addGuiComponents()</code>: This method sets up the GUI components, including a display field for showing numbers and results, and buttons for number input and arithmetic operations. It also sets up the layout using <code>SpringLayout</code> and adds event handling for button clicks.</li>

  <li><code>getButtonLabel(int buttonIndex)</code>: This method returns the label for the buttons based on the button index.</li>

  <li><code>actionPerformed(ActionEvent e)</code>: This method handles button click events and performs the corresponding arithmetic calculations.</li>
</ul>

<h3>3. CalculatorService.java</h3>

<p>This class provides the actual arithmetic calculations for the application.</p>

<h4>Methods</h4>
<ul>
  <li><code>setMathSymbol(char mathSymbol)</code>: Sets the mathematical symbol for the arithmetic operation.</li>

  <li><code>setNum1(double num1)</code>: Sets the first operand for the arithmetic operation.</li>

  <li><code>setNum2(double num2)</code>: Sets the second operand for the arithmetic operation.</li>

  <li><code>add()</code>: Performs addition and returns the result.</li>

  <li><code>subtract()</code>: Performs subtraction and returns the result.</li>

  <li><code>multiply()</code>: Performs multiplication and returns the result.</li>

  <li><code>divide()</code>: Performs division and returns the result.</li>
</ul>

<h3>4. CommonConstants.java</h3>

<p>This class contains common constants used in the application.</p>

<h4>Constants</h4>
<ul>
  <li><code>APP_NAME</code>: Represents the name of the application.</li>
  <li><code>APP_SIZE</code>: Represents the size of the main GUI window as an array of two integers: width and height.</li>
  <li><code>TEXTFIELD_LENGTH</code>: Represents the length of the display field.</li>
  <li><code>TEXTFIELD_FONTSIZE</code>: Represents the font size of the display field.</li>
  <li><code>TEXTFIELD_SPRINGLAYOUT_NORTHPAD</code>: Represents the north padding of the display field in the layout.</li>
  <li><code>TEXTFIELD_SPRINGLAYOUT_WESTPAD</code>: Represents the west padding of the display field in the layout.</li>
  <li><code>BUTTON_ROWCOUNT</code>: Represents the number of rows for the button grid.</li>
  <li><code>BUTTON_COLCOUNT</code>: Represents the number of columns for the button grid.</li>
  <li><code>BUTTON_COUNT</code>: Represents the total number of buttons.</li>
  <li><code>BUTTON_FONTSIZE</code>: Represents the font size of the buttons.</li>
  <li><code>BUTTON_SPRINGLAYOUT_NORTHPAD</code>: Represents the north padding of the button panel in the layout.</li>
  <li><code>BUTTON_SPRINGLAYOUT_WESTPAD</code>: Represents the west padding of the button panel in the layout.</li>
  <li><code>BUTTON_HGAP</code>: Represents the horizontal gap between buttons in the grid layout.</li>
  <li><code>BUTTON_VGAP</code>: Represents the vertical gap between buttons in the grid layout.</li>
</ul>
