# Software Engineering Portfolio
This repository contains the source code and UML diagrams for a software engineering project. The project aims to develop a software application or system using software engineering principles and practices.

## Projects 

### Project 1: [Medical Clinic](https://github.com/xkyleann/Java_Portfolio/tree/main/OOP_Physics)
Description: The business goal of the project is to provide the User with the possibility of contacting a medical clinic to arrange a visit/medical consultation in a way that does not require telephone contact with the clinic. This will reduce the number of calls, which will shorten the waiting time for a connection with a clinic employee and will also increase the quality of services provided. Aim is making diagrams to understand system better.

<details>
<summary><b>1. Glossary of Terms </b></summary>
<table>
  <tr>
    <th> Concept</th>
    <th> Description </th>
  </tr>
  <tr>
    <td>User</td>
    <td>A customer with a profile in the application.</td>
  </tr>
   <tr>
    <td>Receptionist</td>
    <td>The person responsible for handling the application on the Administrator's side.</td>
  </tr>
   <tr>
    <td>Administrator</td>
    <td>The entity that owns the application.</td>
  </tr>
  <tr>
    <td>Chat</td>
    <td>Functionality for electronic communication between the User and the Administrator.</td>
  </tr>
   <tr>
    <td>Ticket</td>
    <td>Commissioned task to be performed for the Registrar.</td>
  </tr>
</table>
</details>

<details>
<summary><b>2. The functional scope of the application for the User </b></summary>
<summary>The solution assumes the provision of a mobile application. The application will be available for Android and iOS, in the versions currently supported by the Google Play and AppStore distribution platforms. After installing the application, the user is registered by providing: </summary>
<ul>
  <li>first name, last name,</li>
  <li>phone number,</li>
  <li>password (repeated).</li>
</ul>
<summary> Registration requires confirmation of the email address by sending an authorisation code to the indicated address. The user is finally registered by entering the correct code from the email received. Login is done using an email address and password. After logging in to which, the user will be able to contact a Receptionist via the "Chat" functionality in order to arrange a visit/consultation without having to contact the clinic by phone. In case of forgetting the password, the User may request a new password using the “I forgot my password”.</summary>
<p>
  <summary><b>2.1 User Profile </b></summary>
</p>
<summary> The user's profile shows his name, surname, ID/PESEL number, contact details such as telephone number and e-mail address, the preferred form of contact and the ability to change the password. You can also add a profile picture. </summary>
 <p><summary><b> 2.2 Menu tab </b></summary></p>
   <summary>The menu of the User app also includes sections such as: </summary>
   <ul>
  <li>How it's working? - it contains the most frequently asked questions about the application along with the answers to them,</li>
  <li>Contact - contains the Administrator's contact details (telephone number, e-mail address)</li>
  <li>Settings - includes access to the "Delete account" tab (where the User can delete an account created in the application), "About the application" (application software version and
number), and links to the Regulations and the Administrator's Privacy Policy.</li>
</ul>
</details>


<details>
<summary><b>3. The functional scope of the administrator application. </b></summary>
<summary> The solution assumes making the administration application available as a Web application. The application can be used by persons - receptionists who register themselves in advance and the system administrator activates their accounts.</summary>
 
  <p><summary><b> 3.1 Authentication model </b></summary></p>
  <summary> Logging in - the process of authentication and authorisation of the Receptionist, consisting in providing the Registrar's ID and authentication password to gain access to use the Application.
Password reminder - functionality that allows you to set a new password for the application in case of its loss </summary>

 <p><summary><b> 3.2 Request list </b></summary></p>
   <summary> After logging in, the Registrar has access to the list of conversations with the Users. The list can be filtered by the following status: </summary>
      <ul>
    <li>Active - a list of notifications not assigned to any Registrar and taken by all Registrars.</li>
    <li>Mine - a list of notifications taken by the logged in Registrar.</li>
    <li>Taken - a list of requests taken by all Receptionists.</li>
    <li>Not picked up - list of requests waiting to be picked up (not assigned to any Registrar).</li>
    </ul>
     <summary>After selecting a single conversation (clicking on a conversation in the list), the current conversation content with the Patient will be displayed in the right part of the screen in the form of a "chat", where the Receptionist can read messages from the Patient and write messages to the Patient himself.</summary>

  <p><summary><b> 3.2 Assigning Tickets </b></summary></p>
    <summary> After selecting the notification, the ticket is automatically assigned to the Receptionist and given the ability to manage it in the menu. If another Receptionist selects an application and then writes a message to the Patient, this will result in assigning the Application to a given Receptionist. </summary>
  
  <p><summary><b> 3.3 Closing a ticket </b></summary></p>
    <summary> The Receptionist conducting the conversation with the Patient, after completing the activities related to the user’s request, may close the ticket by clicking on the “Close” button. In the view of the User's mobile application, a fragment of the conversation will be graphically separated from other messages. </summary>
 
 