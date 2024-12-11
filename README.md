# HelloWorld JavaFX Application

This is a simple JavaFX application. Below are the instructions for setting up, compiling, and running the project.

## Setting up JavaFX

1. Download the JavaFX SDK from the official website:
    - [JavaFX SDK 23.0.1](https://openjfx.io/)

2. Extract the archive to a convenient location. For example:
   ```bash
   /Users/your_user/Development/libs/javafx-sdk-23.0.1
   ```
3. Add JavaFX to your environment using an environment variable.
Open your terminal and run the command:
```
nano ~/.zshrc
```
4. Add the following line to the .zshrc file:
```
export PATH_TO_FX=/Users/your_user/Development/libs/javafx-sdk-23.0.1/lib
```
5. Apply the changes:
```
source ~/.zshrc
```
6. Verify that the PATH_TO_FX environment variable is set correctly:
``` 
echo $PATH_TO_FX
```
7. You should see the path to your JavaFX SDK, for example:
```
/Users/your_user/Development/libs/javafx-sdk-23.0.1/lib
```
## Building the Project with Maven
To build the project using Maven, run the following command:
```
mvn clean package
```

## Running the JavaFX Application
After compilation, you can run the application with this command:
```
java --module-path $PATH_TO_FX --add-modules javafx.controls -cp target/classes org.example.HelloWorld
```
This command tells Java where to find the JavaFX libraries and runs your application.

## This should run your JavaFX application.
Save this file as `README.md` in the root directory of your project. This file contains instructions for setting up JavaFX, compiling, and running your project.
