These two folders contain examples of using Hadoop and Spark for Data processing. These are just examples, you will need Hadoop and Spark to run these.

How to setup:

***To Be Done First***

**ASSUMING YOU HAVE DOWNLOADED HADOOP AND SPARK**

Set an environment variable:
HADOOP_HOME to point to the full path of hadoop-2.7.1
(This is system dependent. Find the way to do that in your system.)

Also, make sure you are using Java 8. 


Now open a terminal (Mac/Linux) or cmd (Windows). 
To try the examples in "hadoop_examples_post" do: 

cd hadoop_examples_post
javac -cp "../spark-2.1.0-bin-hadoop2.7/jars/*" -d bin src/*.java
 (Older version of Windows: change / to \)

One example is: 
  Mac/Linux
java -cp "../spark-2.1.0-bin-hadoop2.7/jars/*":bin MaxTemperature
  Windows:
java -cp "../spark-2.1.0-bin-hadoop2.7/jars/*";bin MaxTemperature

MaxTemperature: 
  reads data from folder "input_weather" and 
  outputs results in "output_weather". 
To see the results, do:
  Mac/Linux:
more output_weather/part-r-00000
  Windows:
more output_weather\part-r-00000

Leave the "hadoop_examples_post" directory by doing: 
cd ..



To try the examples in "SparkJava8Examples_post" do:

cd SparkJava8Examples_post
javac -cp "../spark-2.1.0-bin-hadoop2.7/jars/*" -d bin src/*.java
 (Older version of Windows: change / to \)

One example is: 
 Mac/Linux:
java -cp "../spark-2.1.0-bin-hadoop2.7/jars/*":bin SimpleAppSpark
 Windows:
java -cp "../spark-2.1.0-bin-hadoop2.7/jars/*";bin SimpleAppSpark

