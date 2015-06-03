# Hygienic-Restaurant-Search
The goal of our project is to take into considerations the inspections and rate the restaurants for every locality in Chicago.
The system would project the list of top ten food safe restaurants of a locality (zip code).


Instructions to run the project
--------------------------------
1. Unzip the file HygieneWeb into the workspace.
2. In the hadoop home directory create a folder called input and place the preprocessed file into it.
3. Create a folder called zip inside hadoopLocation/bin/hadoop 
4. Go to the file HygieneWeb/Java Resources/src/FoodInspec.java and change the following line 
(line number 50)
String hadoopLocation = "/home/asim/Softwares/hadoop-1.0.3" to your hadoop home directory
(line number 51)
String desktop = "/home/asim/Desktop"; to your Desktop path
5. Run the project on the Tomcat server
6. The index.jsp page will be displayed and enter a valid zipcode of Chicago.

Note: When running the project for the second time please execute the following commands and delete final.txt and temp.txt from your desktop
sudo ./bin/hadoop fs -rmr zip/temp.txt
sudo ./bin/hadoop fs -rmr out*
sudo ./bin/hadoop fs -rmr final.txt


To preprocess the input data (optional)
1. Place the input file "input.txt" into the workspace and give its path ("input/input.txt") in the command line
2. The processed file will be generated in the workspace as output.txt which the required input file for our project
