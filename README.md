# Movies API Project

## Introduction

This is a personal project I am undertaking as a refresher course to solidify FullStack development skills.

### Technology Stack

### Instructions

1. Install the latest JDK version - https://www.oracle.com/java/technologies/downloads/
2. Create an account or sign in at https://www.mongodb.com/atlas
3. Create an Organization in the portal.
4. Create new Project.
5. Click on the "Build a Database" button.
   - Because the size of the database is small we can create a shared database and select AWS as the provider.
   - Select a region that is closest to you.
   - Select the free tier.
   - Name the cluster.
   - Create cluster.
   - You will be prompted to create a username and password if you don't already have one.
   - When prompted add your IP to the IP Access list. You can allow access to anyone by assigning 0.0.0.0/0 to the IP Address field.
6. Once that is provisioned you will have to connect the database using a client like MongoDB Compass or any other method if you are familiar with it.
   - I will using MongoDB Compass in this tutorial.
   - Click the Connect button and choose MongoDB Compass in the menu.
   - Choose the right system and download the desktop version of MongoDB Compass.
   - Start the program once it is installed.
   - Copy the connection string provided in the website and paste it in the URI box. Make sure to replace the <password> with the password you created.
   - Click save and connect.
7. Open up MongoDB Compass and create a new database. Note: You don't have you mess with the default databases.
   - Name your database and the collection and create your database.
   - Download the following database - https://github.com/fhsinchy/movieist/tree/master/_data
   - Import it through MongoDB Compass, choosing the JSON format and checking "Stop on errors".
8. Intialize Spring Boot using SpringInitializer - https://start.spring.io/
   - Pick Java as language and Maven as the build automation tool.
   - Use the 3.0.5 or the latest stable version.
   - Fill project Metadata:
     - Group is your domain in reverse or it can be any unique domain name.
     - Give an artifact, name, and description.
     - Use Jar as packaging type format
     - Select the Java version installed.
   - Add Dependencies (Hold ctrl for multiple adds)
     - Lombok
     - Spring Web
     - Spring Data MongoDB
     - Spring Boot DevTools
   - Click generate.
9. Extract the downloded zip file and move it to the project folder.