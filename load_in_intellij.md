Here we're going to import the Petclinic project to IntelliJ so you can edit away.

Open IntelliJ.  If you're already in a project go to File -> Close Project.

You should be at the "Create New Project", "Import Project", "Open", etc... menu.


(1) Import Project

(2) Choose the spring-petclinic folder you just downloaded.

(2) Import project from external model, choose Maven.

* Maven is a java build and dependency tool used to compile java, install java dependencies (ie. other packages), run tests, etc.
* The Maven way of organizing a bunch of code is in a “project”. A project may contain one or more java packages.
* All Maven info is found in the pom.xml which lies in the top directory of the Maven “project”.

(3) Keep all the defaults checked but in addition, check "Import Maven projects automatically".

(4) Choose the petclinic project… should already be highlighted. Next...

(5) Select a JDK (java development kit).  Add new if one does not already show.  You should probably only have one JDK on your machine, but maybe not.  Choose the JDK that you downloaded
(Mine is here: `/Library/Java/JavaVirtualMachines/jdk1.8.0_112.jdk/Contents/Home` but yours is probably different on Windows.

(6) name it whatever or keep the default name.

Forge ahead, everything should set up after a few moments and you should be able to browse around the code.

In java, the convention is keeping your packages in src -> main -> java, then the name of the package.  So that's where you'll find all relevent code for the web server.

Last important step is debugging ->


