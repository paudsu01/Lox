# Jlox<sup>*</sup>

JLox<sup>*</sup> is a tree walk interpreter for Lox written in Java. Lox is a full-featured, efficient scripting language from Robert Nystrom's book, [Crafting Interpreters](https://craftinginterpreters.com/). <br>

This project was done as part of my [CS375 independent study](https://github.com/user-attachments/files/18216055/CS375_Fall_2024_Report.pdf) for FA 2024.

The documentation for the Lox programming language itself can be found [here](https://craftinginterpreters.com/the-lox-language.html).

## Requirements

* Java

## Why Jlox<sup>*</sup> and not Jlox ?

While most of my implementation follows the guidelines for the Lox language, there are a few things(features) not part of the actual Lox language that Jlox<sup>*</sup> supports:
* Native functions: `input`, `clock` and `number`.<br><br>
  > `input`: Calling this native function will read a string from standard input.<br>
  > `clock`: Calling this native function will return the current time in seconds.<br>
  > `number`: Calling this native function will convert the argument provided to number, if possible.
* String and number concatenation
* Static methods for classes
> Check [sampleFiles/staticMethods.lox](sampleFiles/staticMethods.lox) file to check out how static methods work in Jlox<sup>*</sup>.

## Installation guide:

* Download the latest version `Lox.jar` file from the releases section here: https://github.com/paudsu01/Lox/releases

## Running the interpreter

* Open up your terminal.
```
cd path/to/directory/of/Lox.jar
```
* To run the interpreter, run:
```
java -jar Lox.jar
```
* To run a .lox file, run:
```
java -jar Lox.jar file.lox
```
> You can also download some sample `.lox` files from the [sampleFiles/](sampleFiles/) directory and run them.

### Running the interpreter from anywhere in the terminal

* I would suggest adding an alias from the terminal to run the `Lox.jar` file such as
  
  ```
  alias jlox="java -jar path/to/Lox.jar"
  ```

  > You can now just type use `jlox` to use the interpreter for the remaining terminal session.

* If you want to add a permanent alias, you can add the command to your shell config file such as `~/.bashrc` file.
