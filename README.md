# REAL-TIME-COLLABORATIVE-DOCUMENT-EDITOR

Company : CODTECH IT SOLUTIONS

Name : Pravin S

Intern Id : CT04DG2370

Domain : WEB DEVELOPMENT

Duration : 4 Weeks

Mentor : Neela Santosh

Description:

This Node.js code sets up a real-time collaborative document editor backend using Express, MongoDB, and Socket.IO. The Express server handles RESTful API routes for creating (POST /documents) and retrieving (GET /documents/:id) documents, which are stored in MongoDB with a unique document ID and content in a JSON format. It uses CORS and JSON middleware to allow cross-origin requests and parse request bodies.

The real-time collaboration feature is powered by Socket.IO. When a client connects and emits a get-document event with a document ID, the server checks the database for that document. If found, it sends the document's content back via load-document and joins the client to a Socket.IO room for that document ID. Any changes made by one client are sent through the send-changes event and broadcast to other clients in the same room using receive-changes. Changes can also be persisted by the client emitting a save-document event, which updates the document in MongoDB.

The server listens on port 3000, enabling collaborative editing where multiple users can simultaneously work on the same document in real time.

Output:

![Image](https://github.com/user-attachments/assets/59d1b1e2-8682-4f8f-a9c7-715bfd97f3b7)

