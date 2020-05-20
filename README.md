How to read a date from the standard application.yaml with Spring Boot.<br/>
<br/>
How to compile and execute :<br/>
mvn package<br/>
java -jar ./target/readADateFromAYamlPropertiesFile-0.0.1-SNAPSHOT.jar<br/>
<br/>
<br/>
---application.yaml<br/>
myDate: 2020-01-01 00:00:00<br/>
---MyConfigurationBean.java<br/>
private Date myDate;<br/>
+getter and setter<br/>
---The class who displays the value of the 'myString' configuration<br/>
@Autowired<br/>
MyConfigurationBean myConf;<br/>
...<br/>
System.out.println(myConf.getMyDate());<br/>
<br/>
<br/>
The application will read the value '2020-01-01 00:00:00' of the property myDate in the standard application.yaml configuration file then display it in the terminal.<br/>


