## Prerequisites

- Python 3.6 or higher

This application uses `tkinter`, which is included in the standard Python library, so no additional installations are necessary.

# Caesar Cipher Tool

This Python application provides a simple graphical user interface (GUI) for encoding and decoding text using the Caesar cipher method.

## Features

- Encode and decode text with a shift value between 1 and 25.
- Simple and user-friendly interface.
- Responsive design that adapts to window resizing.

## Dependencies

- Python 3
- Tkinter library (usually comes with Python)

## Usage

Run the script in your Python environment. The GUI will appear with input fields for text and shift value, along with radio buttons to select between encoding and decoding.

1. Enter the text you want to encode or decode in the 'Text' field.
2. Select the shift value (1-25) using the spinbox.
3. Choose 'Encode' or 'Decode' to set the desired operation.
4. Click 'Apply' to execute the operation and the output will be displayed in the 'Output' field.

## Custom Input Widget

The `InputWidget` class extends the `tk.Frame` class and provides input fields for the text and shift value. 

- The text field allows the user to input the string they want to process.
- The shift value spinbox allows the user to select a number between 1 and 25, representing the shift in the Caesar cipher.

## Custom Result Widget

The `ResultWidget` class also extends the `tk.Frame` class and displays the output of the cipher operation in a read-only entry widget.

## CipherGUI

The `CipherGUI` class is the main application window and contains the logic for the Caesar cipher. It handles user interactions and performs the cipher operation based on the selected mode (encode/decode).

## Caesar Cipher Logic

The Caesar cipher logic is implemented in the `caesar_cipher` method of the `CipherGUI` class. It shifts the letters of the input text by the specified shift value to encode or decode the text.

## Applying the Cipher

The `apply` method is triggered when the user clicks the 'Apply' button. It retrieves the input from the user, calls the `caesar_cipher` method with the appropriate parameters, and displays the result.

## Running the Application

Ensure you have Python installed on your system. Clone or download the repository and run the script:

```bash
python caesar_cipher_tool.py
