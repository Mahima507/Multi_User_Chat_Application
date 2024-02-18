# MultiUser_Chat_App

# Create the User Registration and Login Functionality:
* Design the registration and login screens using Swing and AWT components with the help of Window Builder.
* Implement the logic to capture user registration details and store them in the MySQL database.
* Implement the login functionality by validating the user credentials against the stored data in the database.
# User Registration:
* Users can register by providing their desired username, full name, password, and other necessary details.
* The registration information is validated, and if valid, it is stored in the MySQL database for future logins.

Screenshot 

# User Login:
* Registered users can log in to the chat application using their username and password.
* The login credentials are verified against the information stored in the MySQL database.
* If the credentials are correct, the user is granted access to the chat interface.

Screenshot 2023-06-29 at 2 29 28 PM

# Develop the Dashboard Screen:
* Design the dashboard screen using Swing and AWT components.
* Provide options for users to log in, register, and access the chat functionality.
* Link the login and registration functionality to the appropriate database operations.

# Chat Interface:
* The chat interface is also designed using Swing and AWT components created with the help of Window Builder.
* It includes features like a text input field, and a chat message display area.
* Users can enter text messages in the input field and send them to the chat room.

# Set up the MySQL Database:
* Install and configure the MySQL database server.
* Create a database to store user information, chat messages, and other relevant data.
* Design the necessary tables and define the appropriate schema.
# Integrate with the MySQL Database:
* Use the MySQL jar connectors and JDBC API to establish a connection between the Java application and the MySQL database.
* Implement the necessary JDBC queries and statements to interact with the database, such as storing and retrieving chat messages, user information, and online status.
# MySQL Integration:
* The application uses JDBC (Java Database Connectivity) to establish a connection with the MySQL database.
* JDBC API provides classes and methods to execute SQL queries, retrieve data, and perform database operations.
* The chat application utilises JDBC to store and retrieve chat messages, update user statuses, and manage user information.
# Updating User Details:
* Provide functionality for users to update their profile and account details.
* Allow users to modify their username, password, or any other relevant information.
* Implement appropriate validation and authentication checks before updating the user details in the MySQL database.
* Update the user interface to reflect the changes in real time after the user updates their details.


# Messaging:
* When a user sends a message, it is displayed in the chat message display area and broadcast to all online users.
* Received messages are retrieved from the MySQL database and displayed in the chat message area for each user.


# Implement the Socket Programming and Server Socket:
* Create a server socket that listens for incoming client connections.
* Accept client connections and spawn a new thread for each client.
* Implement the necessary communication protocols using socket programming to enable message exchange between clients and the server.
# Implement the Handshaking Process:
* Define the handshaking process between the client and the server to establish secure communication.
* Encrypt the password on the client side before sending it to the server.
* Validate the credentials on the server side by comparing the hashed password with the stored hashed value.
# Implement Multi-Threading:
* Use multi-threading to handle multiple client connections concurrently.
* Each client connection should be assigned a separate thread to enable independent communication.
# Implement Message Broadcasting:
* When a client sends a message, the server should receive it and broadcast it to all other connected clients.
* Utilise the output streams of each client's thread to send the message to all connected clients.
# Implement Read/Write Data on Stream:
* Use input and output streams to facilitate the exchange of messages between clients and the server.
* Continuously read from the input streams to receive messages from clients.
* Write the received messages to the output streams of other connected clients to broadcast the messages.
# Implement Password Hashing:
* Use a cryptographic algorithm (e.g., MD5, SHA-256) to hash the passwords before storing them in the MySQL database. I have used the MD5 algorithm.
* To authenticate users, compare the hashed password with the stored hashed value during the handshaking process.
# Error Handling and Exception Management:
* Implement proper error handling and exception management throughout the application.
* Display informative error messages to users in case of connection failures, database errors, or other exceptional scenarios.
* Log errors and exceptions for troubleshooting and debugging purposes.
# Private Messaging:
* Implement functionality for users to send private messages to specific individuals.
* Provide options to select the recipient from the user list or by entering the username.
* Ensure that only the intended recipient can view the private message.

# This is a comprehensive project let's break down the different components and their functionalities:
Java: The project is built using the Java programming language, which provides a robust and platform-independent development environment.

Swing and AWT: Swing and AWT are Java's GUI libraries used for creating the graphical user interface of the chat application. They provide components like buttons, text fields, labels, etc., to design the user interface.

MySQL Database: MySQL is a popular open-source relational database management system. In this project, MySQL is used to store user credentials, chat messages, and other relevant data.

Window Builder: Window Builder is a plugin for Eclipse IDE that allows for drag-and-drop GUI development. It simplifies the process of designing the user interface by providing visual tools.

MySQL jar connectors: You need JDBC drivers to establish a connection between the Java application and the MySQL database. These drivers, commonly provided in the form of JAR files, allow the Java application to communicate with the database, execute queries, and retrieve data.

JDBC API using Type-4 Drivers Wrapper: JDBC (Java Database Connectivity) is a Java API that provides a standard way to interact with databases. Type-4 Drivers Wrapper, written in Pure Java Native Driver, allows the Java application to communicate with the MySQL database using the JDBC API.

Driver class for connecting Swing to the Database: A driver class, typically written in C/C++, is used to bridge the gap between the Swing GUI and the database. It acts as a connector, enabling the Swing application to interact with the database using the JDBC API.

Dashboard Screen: The dashboard screen serves as the main interface for users to log in, register, and access the chat functionality. It provides options for users to enter their credentials or create a new account.

Socket Programming: Socket programming is used for communication between the client and server. It allows data to be transmitted over the network using TCP/IP protocols.

Server Socket: The server socket handles incoming client connections. It listens to client requests and establishes a separate thread to handle each client's communication.

Client-side Implementation: On the client side, the chat application consists of a graphical user interface (GUI) built using Swing and AWT. The GUI provides components such as text fields, buttons, and chat message display areas for users to interact with the application. Users can enter their messages in the text field, click a "Send" button to transmit the message to the server, and view received messages in the chat message display area.

Server-side Implementation: On the server side, the chat application utilises socket programming to establish a server socket that listens for incoming client connections. When a client connects, the server creates a new thread to handle communication with that client, allowing multiple clients to connect concurrently. Each client thread maintains its own input and output streams for reading and writing data.

Handshaking Process: When a user logs in or registers, a handshaking process takes place between the client (user) and the server. This process establishes a secure connection and verifies the user's identity.

Password Hashing: Password Hashing is a technique used to secure user passwords by converting them into irreversible hash values. It ensures that the original passwords cannot be easily retrieved even if the database is compromised.

MySQL Database Integration: The chat application employs JDBC to connect to the MySQL database. It utilises the MySQL jar connectors and JDBC API to execute SQL queries, retrieve data, and perform database operations. The application interacts with the database to store and retrieve chat messages, user information, and online status.

Multi-Threading: Multi-Threading is used to manage multiple users simultaneously. Each client connection is assigned to a separate thread, allowing concurrent communication with multiple users.

Read/Write data on stream: The chat application enables users to send and receive messages. Reading and writing data on the stream facilitates the message exchange between clients and the server.

Broadcasting messages: When a user sends a message, the server broadcasts it to all connected clients. This ensures that all users in the chat room receive the message.
