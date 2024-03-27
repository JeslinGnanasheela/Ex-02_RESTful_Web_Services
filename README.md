# Ex-02_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
![image](https://github.com/JeslinGnanasheela/Ex-02_RESTful_Web_Services/assets/119393038/6f9a4a25-1833-4272-9251-7dab84b2e09a)

Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.




Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 
 ![image](https://github.com/JeslinGnanasheela/Ex-02_RESTful_Web_Services/assets/119393038/38dd2e0a-54db-47e0-bb79-6bfe323078f7)



Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.
![image](https://github.com/JeslinGnanasheela/Ex-02_RESTful_Web_Services/assets/119393038/29d5aecb-5318-46cf-9aec-5409e1a08ca0)


Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
![image](https://github.com/JeslinGnanasheela/Ex-02_RESTful_Web_Services/assets/119393038/ea791778-63d5-496e-aea2-8d846b37d14d)

Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
 

 


Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).
![image](https://github.com/JeslinGnanasheela/Ex-02_RESTful_Web_Services/assets/119393038/7f8d98c0-3a8c-4aa5-8b4c-69271fa3697c)



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.




Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. Step 4: Carefully select your RESTful resource (web service) and click OK.
![image](https://github.com/JeslinGnanasheela/Ex-02_RESTful_Web_Services/assets/119393038/fb1dfeb4-ceb7-4983-aab2-f6567423ba95)
 
 


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.
![image](https://github.com/JeslinGnanasheela/Ex-02_RESTful_Web_Services/assets/119393038/f26d4a79-6307-477c-af45-7858e1365bd8)


Step 6: An editing tab will open. Alter getHtml() method with the following.
![image](https://github.com/JeslinGnanasheela/Ex-02_RESTful_Web_Services/assets/119393038/b19862e1-256e-4ee3-9c15-6c55b0e92b71)
 
 


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.
![image](https://github.com/JeslinGnanasheela/Ex-02_RESTful_Web_Services/assets/119393038/453fffee-ed95-47c3-8637-d2763ed776da)


Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
![image](https://github.com/JeslinGnanasheela/Ex-02_RESTful_Web_Services/assets/119393038/edaddd00-f8db-4f67-89bb-f048dfd1acda)
 
 


Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.
![image](https://github.com/JeslinGnanasheela/Ex-02_RESTful_Web_Services/assets/119393038/0ec0643b-ec90-4ce4-bf2b-f9556b792428)


Step 11: Save the project and build it.
![image](https://github.com/JeslinGnanasheela/Ex-02_RESTful_Web_Services/assets/119393038/bb9850ef-864b-4f13-8351-93cc80179482)

Step 12: Run the JSP file and you should see the output in a new browser window.
 
 


Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
