# README #



### WekaProgram purpose ###

A program to calculate the expected values of a dataset while using machine learning. The program uses a J48 model that is tuned to be best fitting for the default dataset. You can run the program with a new file containing instances that needs to be classified or let the program run with the default dataset. 


## usage

The application can be started by calling the jar file on the command line. 
enter the path in which the WekaRunner is stored.
command line:

java build/libs/Wekaprogram-1.0-SNAPSHOT.jar

Then there is a option for using your own arff file containing data with instances that need to be classified

-f <path/to/file/data.arff> 

java -jar build/libs/Wekaprogram-1.0-SNAPSHOT.jar -f (your own file)
 
 
if no file is chosen the program will be run with a example data file that is located in testdata folder 
'testdata/Clean_data_smoking_status_unknown_full.arff'


This is the file containing the unknown, yet to be classified instances.
And a file that contains the instances to be classified.

Running the program will show in the terminal the unclassified unknown instances, and after that the new labelled instances. 

If you chose to classify your own arff file with unknown instances, then after running the program will make a CSV files stored in the folder src/main/resources.
This is a comma separated file with a header so its easy to use for further research in your own environment 


## Dependencies

| Project              | Home Page                                           |
|----------------------|-----------------------------------------------------|
| Java 14.0            | <https://docs.oracle.com/en/java/javase/14/>        |
| apace CLI  1.4       | <https://commons.apache.org/proper/commons-cli/>    |
| weka API  3.8.4      | <https://waikato.github.io/weka-wiki/using_the_api/>|

further dependencies can be found in the build.gradle


### Who do I talk to? ###

for questions contact:
k.reijntjens@st.hanze.nl
