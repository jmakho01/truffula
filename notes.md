# Truffula Notes
As part of Wave 0, please fill out notes for each of the below files. They are in the order I recommend you go through them. A few bullet points for each file is enough. You don't need to have a perfect understanding of everything, but you should work to gain an idea of how the project is structured and what you'll need to implement. Note that there are programming techniques used here that we have not covered in class! You will need to do some light research around things like enums and and `java.io.File`.

PLEASE MAKE FREQUENT COMMITS AS YOU FILL OUT THIS FILE.

## App.java

- the main program that runs everything else
- explains how to use the program, arguments, and examples
- needs to implement TruffulaOptions object, pass into TruffulaPrinter, then call printTree on it

## ConsoleColor.java

- Class composed of enums that represent ANSI escape codes for various text colors on the console
- The code is constructed and returned as a String to be used in the console

## ColorPrinter.java / ColorPrinterTest.java

- Class used in conjunction with ColorConsole to print colored text to the console
- Need to implement print(String message, boolean reset) method
- Test file shows example of how ColorPrinter works

## TruffulaOptions.java / TruffulaOptionsTest.java

- Program that defines configuration options in displaying directory trees, used in App.java
- Shows argument flags, examples of usage, and error exceptions 
- Need to implement TruffulaOptions(String[] args) method
- Test file shows example of how TruffulaOptions works

## TruffulaPrinter.java / TruffulaPrinterTest.java

- Program that is responisble for printing the directory tree itself
- Need to implement printTree() method (multiple waves for this method!)
- Test file has tests that check which OS is running, creating hidden files, and printing trees

## AlphabeticalFileSorter.java