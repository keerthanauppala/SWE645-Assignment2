AUTHOR: KEERTHANA UPPALA

AWS S3 URL of my homepage `http://swe645-hw1-keerthana.s3-website-us-east-1.amazonaws.com`

URL of application (Student survey form ) deployed on EC2: `http://ec2-54-237-219-10.compute-1.amazonaws.com/Keerthana-SWE645-HW1/`

**Software/Technologies Required:**

1. Apache Tomcat 10.0.2 for deploying .war file
2. Java latest version
3. Eclipse IDE for Java EE Developers

**Installation and Setup instructions**

**Java SE - Latest version** 
In order for the assignment to operate properly, the Java Runtime Environment (JRE), Standard Edition (SE) is required. To install JRE to your machine: 
1. Go to `http://www.oracle.com/technetwork/java/javase/downloads/index.html`, or search for Java SE on the Oracle Website. You should see download options available for Java of latest version. 
2. Select the "Download" hyperlink for Java of latest version, and click JRE download. Select the 32-bit or 64-bit executable file (.exe) for your appropriate operating system (OS). 
3. Accept the agreement if needed, and then download the file. 
4. Once the download is complete, run the executable file and follow the on-screen prompts. The JRE should be installed onto the appropriate Programs file in your file system. 
5. Set up the JAVA_HOME environment variable that points to path of your JDK installation
   -For example: JAVA_HOME=c:\Java\jdk1.7

Alternatively, you can also download the Java Development Kit (JDK), which comes with the aforementioned JRE, if you need to create and compile code. To do this, download the appropriate JDK version noted in Step 1 and follow the prompts. 

Please ensure the Java Runtime Environment is installed on the machine. To check, go to the Command Prompt, and then type "java" to the shell and then press ENTER. If there are commands listed (for Java), the installation should be successful. You can also check the version with **"java -version"**. 

**Tomcat 10.0.2**
To download the server to the local machine: 
1. Go to `https://tomcat.apache.org/download-10.cgi`, or search for Tomcat Apache.  
2. Download and save the zip file (under Core bullet) - either the 32-bit or 64-bit depending on your OS.
3. Once saved, unzip and extract the file. You should unzip the installation files in a location that you can easily access. 
4. Once unzipped, select the "tomcat10.0.2" folder, then "apache-tomcat-10.0.2", and then the "bin" directory. You should see startup/shutdown scripts. 
5. Once tomcat is started, open your web browser, and type in `http://localhost:8080` to verify that Tomcat has been successfully installed. 
6. Ensure the "webapps" folder is available from "apache-tomcat-10.0.2" folder. This is necessary to deploy the .war files included in the assignment submission. 

Note that tomcat will be up and running at http://localhost:8080 once successfully downloaded and installed in most instances. You should use the latest version if available.

**Deploying .war file in Tomcat**
1. Extract the Keerthana-SWE645-HW1.zip file which contains .war file, zip file of assignment and README file
2. Place the Keerthana-SWE645-HW1.war file in the webapps folder of Tomcat (Apache Software Foundation\Tomcat 10.0.2\webapps\)
3. Start the tomcat server in the command line (Check whether java is set up in environmental variables)
4. The War file will be extracted in the Apache Software Foundation\Tomcat 10.0.2\webapps
5. Then we can observe the result of the backend using the `http://localhost:8080/Keerthana-SWE645-HW1`. **Please use tomcat port as 8080**

**Eclipse IDE for Enterprise Java Developers**
1. Go to `https://www.eclipse.org/downloads/packages/`, or search for eclipse.org.
2. Download the latest Enterprise Edition of Eclipse IDE - either the 32-bit or 64-bit depending on your OS.
3. Once saved, unzip and extract the file. You should unzip the installation files in a location that you can easily access.
4. Extract the Keerthana-SWE645-HW1.zip file and open the SWE645-HW1 folder using Eclipse
5. Configure Tomcat in Eclipse, if there is no tomcat server on the servers tab
   * R-click in the space under Servers tab and select New to define new server – select Tomcat
   * R-click on the Tomcat server and select Start
   * Once the server is running, you can access the homepage at localhost:8080
6. Trouble shooting steps
   * If you don’t see the Server tab in the bottom portion of the Eclipse IDE, do the following:
     – Window-> Show View -> Other - > Servers
   * Once the server is started, you can test by going to localhost:8080
   * If you get HTTP Status 404 – page not found error, do the following two things:
     - R-click on the Tomcat v7.0 Server and select Properties, and press the button “Switch Location” so that the Location is changed from “Workspace Metadata” to “/Servers/Tomcat Server v7.0 at localhost server [STEP 1]
     - Double click on the Tomcat v7.0 Server and for the server location make sure use select radio button for “Use Tomcat Installation” and NOT the “Use workspace metadata” [STEP 2]
     - Now Save the changes or try deleting the page with newly selected radio button option, it will ask you to save the settings, if so, select Yes
     - Restart the server and now you should be able to see the tomcat startup page at localhost:8080
   
