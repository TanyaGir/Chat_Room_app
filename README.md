# Chat Room 
## Introdution
This application is a simple chat room application developed using web-sockets in Java. The basic tasks users can perform are:

- entering a room
- sending messages
- leaving the room

# Websocket
WebSocket is a communication protocol that makes it possible to establish a two-way communication channel between a server and a client.

# Java Classes

# Message.Java
Message is a model class. It is the message payload that will be exchanged between the client and the server.

# WebSocketChatServer.java
WebSocketChatServer is the controller class. It has below method implementations:

- onOpen:Establishes a connection between client and server
- onMessage: Gets session and user information and sends messages.
- sendMessageToAll: Sends the message to all connected users
- onClose:Closes the connection

# WebSocketConfig.java
WebSocketConfig is the web socket configuration file which defines server endpoint exporter

# LoginController.java
LoginController is controller file to implement the login functionality and render the chat url

# WebSocketChatApplication.java
WebSocketChatApplication is the main class to boot the application

# login.html
This view-page helps the user to login.

# chat.html
This view-page shows the chat window where user can also type-in his\her message

# pom.xml
Its the maven build file with dependency on spring-boot-starter-web, spring-boot-starter-websocket, spring-boot-starter-thymeleaf, jquery, fastjson.
