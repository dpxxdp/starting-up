spring-petclinic is a sample web server written in Java. it uses Tomcat, SpringMVC, Hibernate, and MySQL. Don't go too deep on any of those yet.  They're all well known and heavily used throughout the java world though.  

Here you're going to download the source code, and then run the server from you local computer.  This allows for tighter development cycle, where you can make changes to the server code and rerun it locally, rather than deploying it up to a real server before seeing the changes.

In your console, change into whichever directory you want to keep the project in.

```
git clone https://github.com/dpxxdp/spring-petclinic.git
```

This cloned the git repository from my github repo down to your local machine.

Change into the directory it just created (spring-petclinic) and then start the server:

```
./mvnw spring-boot:run
```

You should be able to see it starting up in the console.  When you get to this line: `Started PetClinicApplication in 30.277 seconds (JVM running for 31.118)`, then go and visit http://localhost:8080/ in your browser.  You should see the application there.  Your browser is making a request to your own port 8080, where your java web application is being served out of.

Next, set up the project in Intellij, and make some edits.

