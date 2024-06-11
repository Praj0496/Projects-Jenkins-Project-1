
<H1>Automated CI Pipeline with Git, Jenkins, and Maven on AWS</H1>


<H3>Project Description:</H3>

This project is a comprehensive implementation of a Continuous Integration (CI) pipeline using Git, Jenkins, and Maven, hosted on an AWS EC2 instance. The primary objective of the project is to automate the build and testing process, thereby enhancing the efficiency of the software development lifecycle.

The project begins with the creation of Java code, which is then stored in a pom.xml file and version-controlled using Git. An EC2 instance with an Ubuntu image is spun up on AWS to host the CI pipeline.

Jenkins, a leading open-source automation server, is installed on the EC2 instance. It is accessed via the instance’s public IP on port 8080. The Jenkins setup includes the installation and configuration of the Maven plugin, which is a powerful project management tool primarily used for Java projects.

A new Maven job is created within Jenkins, with the Source Code Management (SCM) system specified as Git. The Git repository and credentials are added to the job configuration, and the pom.xml file is updated as the code file. The build stage in Maven is set as ‘package’.

In addition, a Git SCM trigger is selected and a Jenkins webhook is created for Git Repo. This setup ensures that any commits or changes pushed to the pom.xml file automatically trigger the Jenkins job. As a result, the Java code is automatically packaged and stored as a .jar file whenever changes are made to the codebase.

This process demonstrates the successful implementation of a CI pipeline, where code changes are automatically built and tested, significantly improving the speed and quality of software development. This project showcases the power of automation in DevOps and its impact on improving the efficiency and reliability of software delivery.
