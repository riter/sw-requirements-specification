## Software Requirements Specification for Balanta

>Prepared by:
>* Juan Carlos Suarez
>* Alfredo Avila Soto 
>* Riter Angel Mamani

# **Table of Contents**

1. [Introduction](#introduction)
2. [Overall Description](#overall-description)
3. [System Features](#system-features)
4. [External Interface Requirements](#external-interface-requirements)
    1. [User Interfaces](#user-interfaces)
    2. [Hardware Interfaces](#hardware-interfaces)
    3. [Software Interfaces](#software-interfaces)
    4. [Communications Interfaces](#communications-interfaces)
5. [Other Nonfunctional Requirements](#other-nonfunctional-requirements)
    1. [Performance Requirements](#performance-requirements)
    2. [Safety Requirements](#safety-requirements)
    3. [Security Requirements](#security-requirements)
    4. [Software Quality Attributes](#software-quality-attributes)
6. [Other Requirements](#other-requirements)

## 1. Introduction
This document details the software requirements for the system of the insurance company "Balanta", based on: the Functional and Non-Functional Specifications and the Supplementary Specifications.

**1.1 Purpose**

The purpose of this document is the specification of the software requirements for the mass marketing system for the insurance company Balanta.

**1.1 Document Conventions**

All the specifications that are detailed in this document have a priority and a risk which are defined according to the importance they have for the client.

**1.2 Intended Audience and Reading Suggestions**

This document will be available to the project manager, developers, evaluators and documentation writers.

This document contains the scope of the project, the references, a general description of the characteristics of the product, operating environment, implementation restrictions, external interface requirements, non-functional requirements, as well as a list of requirements with their respective valuation. In this way, it will be possible to specify and prioritize those requirements to carry out the development of the system, therefore this document must be known by all the people involved in the development process.

**1.3 Project Scope**

This is a massive marketing system, which allows sending emails to all the company's clients, it also allows to segment the data of these clients to have a specific scope for each type of client, users can also modify the templates used at the time. to send emails allowing to customize automatic shipments.


## 2. Overall Description

**2.1 Product Perspective**

This product arises from the lack of a massive marketing system that allows them to have faster access to their customers.

**2.2 Product Features**

This product is a massive marketing system that will allow them to send emails to all their clients in a faster and more segmented way, so that they can better reach each client and types of clients.

**2.3 User Classes and Characteristics**

The following classes of users will participate in this product: The person in charge of the product on the client's side, the person in charge of the development, as well as all the team that will be in charge of product development.

**2.4 Operating Environment**

For this product we do not have a specification of what the customer wants or has available to be able to host the product.

**2.5 Design and Implementation Constraints**

The main limitations we have to develop this product is the lack of knowledge of the resources available to the company Balanta.

**2.6 User Documentation**

For the correct handling of part of the final users for this product it will be necessary to deliver to the people in charge of the product of the company Balanta documentation in which will have a user guide to be able to operate the system in an appropriate way, this in addition to the respective instruction.

### **3.1 Feature 001 Sending personalized emails**
 
```
3.1.1. Description and Priority
    It allows creating emails with personalized content based on the information of customers and potential customers.
    Priority: High
    Risk: 8  
    
3.1.2. Stimulus/Response Sequences
    * The user enters the Mail Marketing section
    * The system displays the Mail Marketing screen where you see a history of all the personalized mails made
    * The user selects the option to send mail again.
    * The system shows you the personalized mail form.
    * The user Fill in the fields 
        o Select group of clients
        o Title of the mail or Content of the Mail
    * Select Send.  
    
3.1.3 Functional Requirements  

    REQ-001: The user must be able to see the listings of all the emails sent through the system and be able to view the details of each email  
    
    REQ-002: The user must be able to create a new email to be sent. You must be able to choose the group of clients to whom you want to send the mail.  
    
    REQ-003: In the content of the mail should be able to insert images, links. You must be able to enter special tags where the system then replaces the customer's data. The tags are% NAME% (customer name)% COMPANY% (company where the client works)% ADDRESS% (customer's address).  
    
    REQ-004: The user must be able to create reply emails and link them to an email, so that it is sent in case the first email is answered and so on in a mail chain.

```    

### **3.2 Feature 002 Customer Portfolio**

```
3.2.1. Description and Priority
    Creation, modification, listing and elimination of Clients.
    Priority: High
    Risk: 8  
    
3.2.2. Stimulus/Response Sequences
    * The user enters the Customer Portfolio section
    * The system displays the Customer Portfolio screen where all the system's clients are listed.
    * The user selects the new customer option
    * The system shows you the registration form
    * The user Fill in the fields 
        o Name
        o Age
        o Address
        o Company
        o Amount of family
        o Diseases
        o Salary
    * Select Save
    * The system shows a pop-up indicating that it has been saved
        
3.2.3 Functional Requirements  
    REQ-001: The user must be able to see the listings of all clients.  
    
    REQ-002: The user must be able to create a new Client by filling in a form with the following fields Name, age, address, company, family size, select list of diseases, Salary.  
    
    REQ-003: The user must be able to modify the information of a client.  
    
    REQ-004: The user must be able to delete a client.  
    
    REQ-005: The user must be able to register clients by batch, loading csv files.

```

### **3.3 Feature 003 Customer Group**

```
3.1.1. Description and Priority
    Creation, modification, listing, elimination of group of clients and assignment of Clients to a group.
    Priority: High
    Risk: 8  
    
3.1.2. Stimulus/Response Sequences
    * The user enters the Customer Group section
    * The system displays the Customer Group screen where all the customer groups of the system are listed.
    * The user selects the new group option.
    * The system shows you the registration form.
    * The user Fill in the fields 
        o Name
    * Select Save
    * The system shows a pop-up indicating that it has been saved.  
    
3.1.3 Functional Requirements  
    REQ-001: The user must be able to see the list of all client groups.  
    
    REQ-002: The user must be able to create a new group by filling in a form with the following Name field.  
    
    REQ-003: The user must be able to modify the information of a client group.  
    
    REQ-004: The user must be able to delete a client group.  
    
    REQ-005: The user must be able to assign clients to a group.  
    
    REQ-006: The user must be able to upload a batch file in csv format to assign clients to a group.  
```

### **3.4 Feature 004 Blog**

```
3.1.1. Description and Priority
    Creation, modification, listing, elimination of blogs.
    Priority: Medium
    Risk: 6 
    
3.1.2. Stimulus/Response Sequences
    * The user enters the blog section.
    * The system displays the blog screen where all the blogs in the system are listed.
    * The user selects the option of new blogs
    * The system shows you the registration form
    * The user Fill in the fields 
        o The user Fill in the fields
        o Blog content
    * Select Save 
    * The system shows a pop-up indicating that it has been saved  
    
3.1.3 Functional Requirements  
    REQ-001: The user must be able to see the list of all blogs including the link with which you can enter the blog externally.
    
    REQ-002: The user must be able to create a new blog by filling in a form with the following fields: Title of the blog, content of the blog.
    
    REQ-003: The user must be able to modify the information of a blog.
    
    REQ-004: The user must be able to delete a blog.
    
    REQ-005: In the content of the blog you must allow inserting images, links, gifs.
    
    REQ-006: The blog must have a comments section which only registered users should be able to comment on.
    
    REQ-007: The blog must have a download section to download extra content. In order to download the content, the client must register on a landing page (Feature 006) and then let him download the content.  
```

### **3.5 Publicaciones a través de la Api de facebook**

```
3.1.1. Description and Priority
    Realization of content publications and promotion using Facebook's api.
    Priority: Low
    Risk: 2
    
3.1.2. Stimulus/Response Sequences
    * The user enters the advertising section for Facebook
    * The system displays the advertising screen for Facebook where you can see a history of all the publications made
    * The user selects the option of new publication.
    * The system shows you the publication form
    * The user Fill in the fields 
        o Advertising title
        o Duration
        o Payment of advertising by life cycle or by number of views. 
        o Payment amount.
        o Content of advertising
    * Select Save 
    * The system shows a pop-up indicating that the publication has been made.
    
3.1.3 Functional Requirements  
    REQ-001: The user must be able to see the listings of all publications made through the system and be able to view the detail of each publication.  
    
    REQ-002: The user must be able to create a new publication, filling in a form with the following fields title of advertising, duration, type of payment of advertising either by life cycle or by number of views, amount of payment and the content of advertising.
  
```

### **3.6 Feature 006 Landing page**

```
3.1.1. Description and Priority
    Customer data registration page.
    Priority: High
    Risk: 9
    
3.1.2. Stimulus/Response Sequences
    * The client enters the landing page page.
    * The system displays the landing page screen.
    * The client Fill in the fields 
        o Name
        o Age
        o Address
        o Company (not mandatory)
        o Amount of family (not mandatory)
        o Diseases (not mandatory)
        o Salary (not mandatory)
    * Select Send 
    * The system forwards it to the page requested by the client.

    
3.1.3 Functional Requirements  
    REQ-001: The client must be able to fill in the fields of name, age, address, company, amount of family, diseases, salary. The required fields are Name, age and address. This data must be registered in the system by creating a client and automatically be assigned to a configurable group.
    
    REQ-002: The landing page must be initialized with a page to be addressed. In case the client registers then he must be redirected.
    
    REQ-003: The landing page must show an option to tag allowing the company to send mail of offers and promotions.
    
    REQ-004: The system must send a personalized email to the clients that register on the landing page.

```

### **3.7 Feature 007 Reports**

```
3.1.1. Description and Priority
    It should generate reports of number of registered customers, number of views of publications, amount of view of blogs, amount of mail sent, number of mails answered.
    Priority: Medium
    Risk: 5
    
3.1.2. Stimulus/Response Sequences
    * The user enters the reports page
    * The system displays the reports screen
    * The user selects the report that he wants to see
    * The user Fill in the fields 
        o Range of dates
    * Select generate 
    * The report with the criteria is displayed
    * Select export and select the type (Excel, pdf)
    * The report is downloaded
    
3.1.3 Functional Requirements  
   REQ-001: Generate a report of the number of registered customers in a certain range of dates.
   
   REQ-002: Generate report of views of publications in a certain range of dates.
   
   REQ-003: Generate report of number of views in blogs in a certain range of dates.
   
   REQ-004: Generate a report on the number of emails sent in a certain range of dates.
   
   REQ-005: Generate a report on the number of mails answered in a certain range of dates.
   
   REQ-006: You must be able to export the reports in Excel or pdf format.
```

## 4. External Interface Requirements

## 4.1 User Interfaces
>Mocku Login

![](/login.png)

>Mockup Menu

![](/menu.png)

The user must create a login page when accessing any page in case he has not done it before. Administrative tasks must have a Ui interface.
The Facebook interface should allow you to send publications without having to log in repeatedly. The e-mail delivery interface must follow these as there may be some error in the shipment.

## 4.2 Hardware Interfaces
All server-side components must execute on server-class computers. All client-side components
must execute on workstation-class and personal-class computers.

## 4.3 Software Interfaces
The software interface must follow the Model-View-Controller (**MVC**) model to render and model data objects. The interface must be able to connect to a database to store the different data of the system. In some cases the source and destination formats must include **HTML** and Comma Separated Value (**CSV**).

## 4.4 Communications Interfaces

The communication architecture must follow the **client-server** model. The communication must be through **HTTP** Secure **(HTTPS)**. 

Between the client and the server must use a web service that complies with REST, both for the web and for communications with other platforms such as Facebook.

## 5 Other Nonfunctional Requirements

## 5.1 Security Requirements
The percentage of error when sending an email must be as small as possible.
Security in the management of customer information since data are handled strictly by people.
