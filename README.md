# Convert-Text-to-Speech-using-Python

# Introduction:
In this project, we will convert the text into speech using Python. It will be made possible by using the gTTS module in Python. It is a Python library and CLI tool to interface to Google Translate Text to speech API. Let’s get into this and make some text to get converted into speech in any language you want.

# Installation: 
o install the GTTS (Google Text-to-Speech) module for Python, you can use the pip package manager by running the following command in your command line or terminal:

$ pip install gtts
This will install the latest version of the GTTS module on your system. You can then use it in your Python script by importing it with the following statement:

$ from gtts import gTTS
Explanation:
The first step is to import the module and with the help of “import” keyword, we will import “gTTS” & “os” libraries for converting the text and playing the audio respectively.

This project can be done in two ways. One, the text can be provided by the user itself in the program. Second, a file can act as text and the whole file can be converted into speech. Let’s discuss both ways.

# First way:
For this, first of all, the user stores the text under any variable, and then they should set the language in which they want to hear. So, ‘my_text’ and ‘language’ are the two variables created in this program to store the text and language type. Here, we want the speech to be in the English language, for this, we have to use the language code “en” for it. One can use anything accordingly.

In the next step, we will pass the text to the gTTS engine using “gTTS(text=, lang=, slow=) “.

In this, the variable in which the text is stored must get passed, the lang is for language, and the slow parameter takes a bool value accordingly if the user wants the output audio to be fast or slow.

Now, “.save(filename)” will request the API to write the result to the file, and with the help of “os. system()” we will interact with our OS for the audio file to be played by passing “start <filename>” as a parameter to the function.

Second way:
For this, there is only one change in place of passing the text, we will open the file in a read mode by using the “open(filename, mode)” function. In this, for reading mode, we will pass “r” as the second parameter.

# Output:

Thus the text is conveted to speech.
