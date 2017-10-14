# What you will need:
Have maven 3.3.3, java jdk8 installed.
Open terminal and Navigate to the folder you have saved the project (You should see the
pom.xml file)
# To run the tests
The command to run the tests is:
mvn clean install -DbrowserName=firefox
or
mvn clean install -DbrowserName=chrome

or from the Eclipse/InteliJ IDE  ( in the run configurations under the VM arguments e.g
-DbrowserName=firefox)

# Important note
The tests were written using firefox version 42.0. The latest version of firefox (48) doesn't currently work with selenium (2.53.0) so don't do any updates before running the tests.
The tests can alternatively run on chrome and on a MAC terminal.
If you want to run on chrome and on WIN7 then go to work/src/main/java/myproject/myproject/WebDriverInit.java and use chromedriver.exe instead ( the executable files are added in src folder). This logic was not added in the code because I was not able to test it locally as I have a MAC

