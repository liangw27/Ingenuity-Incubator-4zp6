# Software Requirements Specification
## For Ingenuity Incubator

Version 0.1<br>
Prepared by Team Aquafina <br>
Weijie Liang -  400180358  <br>
Kexin Liu -    <br>
Shanghong Shen -     <br>
Liyang Wang -   <br>
Fang Ye - 400273067     <br>
**Instructor** : Dr. Jacques Carette    <br>
**Course** : COMPSCI 4ZP6     <br>
**Date** : 2020-10-08     <br>

Table of Contents
=================
* [Revision History](#revision-history)
* 1 [Introduction](#1-introduction)
  * 1.1 [Document Purpose](#11-document-purpose)
  * 1.2 [Product Scope](#12-product-scope)
  * 1.3 [Definitions, Acronyms and Abbreviations](#13-definitions-acronyms-and-abbreviations)
  * 1.4 [References](#14-references)
  * 1.5 [Document Overview](#15-document-overview)
* 2 [Product Overview](#2-product-overview)
  * 2.1 [Product Perspective](#21-product-perspective)
  * 2.2 [Product Functions](#22-product-functions)
  * 2.3 [Product Constraints](#23-product-constraints)
  * 2.4 [User Characteristics](#24-user-characteristics)
  * 2.5 [Assumptions and Dependencies](#25-assumptions-and-dependencies)
  * 2.6 [Apportioning of Requirements](#26-apportioning-of-requirements)
* 3 [Requirements](#3-requirements)
  * 3.1 [External Interfaces](#31-external-interfaces)
    * 3.1.1 [User Interfaces](#311-user-interfaces)
    * 3.1.2 [Hardware Interfaces](#312-hardware-interfaces)
    * 3.1.3 [Software Interfaces](#313-software-interfaces)
  * 3.2 [Functional](#32-functional)
  * 3.3 [Quality of Service](#33-quality-of-service)
    * 3.3.1 [Performance](#331-performance)
    * 3.3.2 [Security](#332-security)
    * 3.3.3 [Reliability](#333-reliability)
    * 3.3.4 [Availability](#334-availability)
  * 3.4 [Compliance](#34-compliance)
  * 3.5 [Design and Implementation](#35-design-and-implementation)
    * 3.5.1 [Installation](#351-installation)
    * 3.5.2 [Distribution](#352-distribution)
    * 3.5.3 [Maintainability](#353-maintainability)
    * 3.5.4 [Reusability](#354-reusability)
    * 3.5.5 [Portability](#355-portability)
    * 3.5.6 [Cost](#356-cost)
    * 3.5.7 [Deadline](#357-deadline)
    * 3.5.8 [Proof of Concept](#358-proof-of-concept)
* 4 [Verification](#4-verification)
* 5 [Appendixes](#5-appendixes)

## Revision History
| Name | Date    | Reason For Changes  | Version   |
| ---- | ------- | ------------------- | --------- |
|      |         |                     |           |
|      |         |                     |           |
|      |         |                     |           |

## 1. Introduction

### 1.1 Document Purpose
This requirement document is for the final year capstone project which is being developed by the team Aquafina.The purpose of this document is to present a detailed description for a new web-based e-commerce system which acts as a community marketplace using virtual currency for Reframery. It will mainly explain the purpose of this web application, the user interfaces and the specific functions of the web application. It also explains the constraints of this software and the expected software quality. 

This document is intended for the following stakeholders:

* **The Instructor for 4ZP6**

Dr. Carette is the instructor for the Computer Science Capstone Project: COMP SCI 4ZP6. Dr Carette designs the requirements and milestones, and will mark all the required documents and the project implementation.  

* **The Teaching Assitants for 4ZP6**

Ethan and Brendan are the teaching assistant for this course, and they will assistant Dr. Carette mark the deliverables, and help students by providing valuable suggestions and feedback.

* **The Client**

The team leaded by Dr. Benson Honig is the client of this project, and they initiatived Reframery which provides entrepreneurship consulting and coaching services for diverse individuals to start new economic activities. Dr. Benson Honig is a professor of Degroote School of Business in McMaster University and the co-founder of regramery and he will focus on how the product will achieve their team mission - supporting diverse individuals and communities. Dr. Ana Cristina Siqueira is also the co-founder of Regramery, and she will focus on the expected product interfaces and functions. Dr. Sandra Moraes and two students in the their team did some research about community currency and they will focus on the technical solutions in this project.

* **The Aquafina**

The Aquafina is composed of five students enrolled in the Computer Science Capstone Project. They are Weijie Liang, Kexin Liu, Shanghong Shen, Liyang Wang and Fang Ye. The team will be responsible for managing the project effectivley and distributing tasks amongst the team members, including requiremnt gathering, documentation, designing, developing and testing.

* **Users**

The target users are diverse individuals who hope to commercialize their products, services and knowledge in the community network, and most the users maybe at the bottom of the pyramid. The web application will be used in Canada, the USA and Brazil in the first stage. Thus, most users will have basic experiences using online transaction system. 

### 1.2 Product Scope

The Ingenuity Incubator is a web-based e-commerce system where people can trade their products and service including knowledge using virtual community currency. Users can create their lists of product or service details in different categories and search the items they needs. The software will record the transaction history and details for the each user and keep track of the balance for currency, products and services. The Ingenuity Incubator system is a part of the Reframery Information System, which aims to integrate the virtural currency based on blockchain and the marketplace application.  

This system will help the diverse individuals to start their commercial actvities in their social network and improve their personal life. People who have competence and creativity will engage in the community well and make their potential contribution to local economies. Thus, it will also plays a positive impact on the community economies during the global economic stagnation. What the web application can do will help the Reframery team to fulfill their mission. The Reframery team can improved their consulting and training service for their client based on the data in the information system. 

### 1.3 Definitions, Acronyms and Abbreviations
RC - currency code for Reframery Currency

\$ - currency symbol for Reframery Currency

### 1.4 References
Reframery. Retrieved Oct 10, 2020, from https://www.reframery.org/ 

jam01/SRS-Template. Retrieved Oct 10, 2020, from https://github.com/jam01/SRS-Template



### 1.5 Document Overview
The outline of this document is based on IEEE 830, and ISO/IEC/IEEE 29148, and the rest of the document contains the detailed specification for the e-commerce system. It is organized as follows: 

* Section 2: Product Overview

It provides a general description for the product perspective, user characteristics, constraints and dependencies which will affect the e-commerce system and its requirements.  Execept that, It also provides a background for the product functions which are described in detail in Section 3 of this document. 

* Section 3: Requiremetns <br>

It decribes the requirements for the external interfaces, functions, quality-related property in detail, which enables designers to design the system and tests to test it to satisfy the requirements. 

* Section 4: Verification <br>

It provides the plan for verification approaches to qualify the system.
* Section 5: Appendixes <br>

## 2. Product Overview

### 2.1 Product Perspective
The Ingenuity Incubator is an electronic commerce software supporting product, service and knowledge trade using the Reframery currency within a community. This system is expected to support a number of functions for both users(buyers and sellers) and the system administrator, and implement client-server model.

The software must be available to users in targetted communities and it must work correctly in different mobile systems, including Android and iOS. 

### 2.2 Product Functions
The Ingenuity Incubator will provide a number of functions:

a. users:
* Users are identified as buyers or sellers.
* Each user has an unique username, a non-restricted password, a non-restricted email address and a physical address.
* Any person within a targetted community can sign up for a new user account.
* Users can access the platform and check their balance and transaction history.

b. currency:
* There is a common-pool fund, which contains overall amount of currency to be assigned.
* Each user is originally assigned to own a number of currency in their wallet.
* The amount of currency involved in each transaction will be recorded.

c. administrator:
* Administrator can validate registration of users.
* Administrator can assign currency to users.
* Administrator can stop any suspicious transactions.
* Administrator can view the history of transactions.

d. products/service/knowledge:
* Products/service/knowledge in the marketplace will be originally listed by alphabetical order.
* Products/service/knowledge can be searched by typing in related descriptive key words.
* Users(sellers) can register,edit and discard their selling products/service/knowledge with detailed descriptions.
* All users can view the lists for products/service/knowledge using filters.
* The system will record purchase/selling history of products/service/knowledge.

### 2.3 Product Constraints
* Initial release can only allow a limited number of products/service/knowledge in research result owing to restrictions by database system.
* Initial release can only be supported on iOS and Andriod system.
* The Ingenuity Incubator can not work without JavaScipt support.
* The Internet connection is also a constraint. Since the app fetches data from the database over the Internet, reliable internet connection is important to make our app bahave functionally.

### 2.4 User Characteristics
There are three kinds of users of The Ingenuity Incubator.
* Users(sellers): These users will access the system most frequently since they need to monitor any requests for products/service/knowledge. They are supposed to provide information on their sales as detailed as possible. Since the majority of sellers have minimal technical knowledge, they may need intuitive navigation aids and simple page layouts. They also need notifications from the software when there are requests for their selling goods.
* Users(buyers): These users will access the system when they seek for products/service/knowledge to satisfy their needs. Since the majority of buyers have minimal technical knowledge, they may need intuitive navigation aids and simple page layouts. They may require the function of searching using key words to fastly identify related products/service/knowledge for sales. They may also require a filter to sort the lists of goods.
* Administrator: They are responsible for maintaining the system of The Ingenuity Incubator and will participate in software fixes, deployment and regular maintenance.

### 2.5 Assumptions and Dependencies
* Users: We have assumed all users have access to their mobile phones and they are capable of operating basic functions of iOS or Andriod system. For example, they are able to install the app from app store and open it using their phones. After that, they are able to register a new account and then login with usernames and passwords.
* Providers: We assumed that the app store of iOS or Andriod system will allow our app to be installed by users.
* Safety: We assumed that there is no hackers attacking our system deliberately.

### 2.6 Apportioning of Requirements
| Requirement Index| Requirement    | software element |
| ----------- | -------------- | ------------------- |
|      R1    |  user - registration  |        name/id,password,email,address              |  
|     R2      |    user - log-in      |        name/id,password          |    
|     R3      |      user - create product/service/knowledge category   |      category name           |    
|     R4      |      user - add a new product/service/knowledge    |      titles, details of product/service/knowledge              |     
|     R5      |      user - edit product/service/knowledge information   |      titles, details of product/service/knowledge              |    
|     R6      |      user - search a product/service/knowledge   |    type-in keywords, titles and details of product/service/knowledge             |   
|     R7      |      user - purchase a product/service/knowledge   |      currency balance, price             |      
|     R8      |  administrator -  place currency to user    |       currency amount, user name/id            |      
|     R9      |  administrator -  approve users' proposal   |    username/id            |     
|     R10      |      record wallet balance   |    currency balance                |     
|     R11     |      record selling   |     currency balance, price              |     
|     R12     |      record purchase   |         currency balance, price             |   
|     R13     |      security - user authentication   |      user email     |    

Requirements that may be delayed until future versions of the system:
* It will have multiple languages versions.
* It will be added support for visually impaired users.
* It will be added the function of online customer service.  

## 3. Requirements
> This section specifies the software product's requirements. Specify all of the software requirements to a level of detail sufficient to enable designers to design a software system to satisfy those requirements, and to enable testers to test that the software system satisfies those requirements.

> The specific requirements should:
* Be uniquely identifiable.
* State the subject of the requirement (e.g., system, software, etc.) and what shall be done.
* Optionally state the conditions and constraints, if any.
* Describe every input (stimulus) into the software system, every output (response) from the software system, and all functions performed by the software system in response to an input or in support of an output.
* Be verifiable (e.g., the requirement realization can be proven to the customer's satisfaction)
* Conform to agreed upon syntax, keywords, and terms.

### 3.1 External Interfaces
> This subsection defines all the inputs into and outputs requirements of the software system. Each interface defined may include the following content:
* Name of item
* Source of input or destination of output
* Valid range, accuracy, and/or tolerance
* Units of measure
* Timing
* Relationships to other inputs/outputs
* Screen formats/organization
* Window formats/organization
* Data formats
* Command formats
* End messages

产品外部的界面都有什么？

#### 3.1.1 User interfaces
The user interface for the ingenuity incubator project has been designed in the early-stage prototype by the client. The application shall inherit its functionality, allowing users to trade products and services using community currency. The user interface shall be simple and focus on usability. The user interface shall be compatible to any browser by which user can access to the product.
> The application should have following user interaces:
* Initial page with the a preview of information such as the name of the community, the number of participants, and the start-up reframery currency
* Main page for selling and buying products. The screen should display the trader's name and the product's price（？）
* Login page for authenticating users. The screen should accept new user registration and login user name and password. (?)


#### 3.1.2 Hardware interfaces
The Ingenuity Incubator application is web-based and has no direct hardware interface.

#### 3.1.3 Software interfaces
The application shall communicate with the internet.
The application shall communicate with user and product database 
The application shall communicate with block chain for community currency.

### 3.2 Functional
> This section specifies the requirements of functional effects that the software-to-be is to have on its environment.

### 3.3 Quality of Service
> This section states additional, quality-related property requirements that the functional effects of the software should present.

#### 3.3.1 Performance
If there are performance requirements for the product under various circumstances, state them here and explain their rationale, to help the developers understand the intent and make suitable design choices. Specify the timing relationships for real time systems. Make such requirements as specific as possible. You may need to state performance requirements for individual functional requirements or features.

#### 3.3.2 Security
Specify any requirements regarding security or privacy issues surrounding use of the product or protection of the data used or created by the product. Define any user identity authentication requirements. Refer to any external policies or regulations containing security issues that affect the product. Define any security or privacy certifications that must be satisfied.

#### 3.3.3 Reliability
Specify the factors required to establish the required reliability of the software system at time of delivery.

#### 3.3.4 Availability
Specify the factors required to guarantee a defined availability level for the entire system such as checkpoint, recovery, and restart.

### 3.4 Compliance
Specify the requirements derived from existing standards or regulations, including:  
* Report format
* Data naming
* Accounting procedures
* Audit tracing

For example, this could specify the requirement for software to trace processing activity. Such traces are needed for some applications to meet minimum regulatory or financial standards. An audit trace requirement may, for example, state that all changes to a payroll database shall be recorded in a trace file with before and after values.

### 3.5 Design and Implementation

#### 3.5.1 Installation
Constraints to ensure that the software-to-be will run smoothly on the target implementation platform.

#### 3.5.2 Distribution
Constraints on software components to fit the geographically distributed structure of the host organization, the distribution of data to be processed, or the distribution of devices to be controlled.

#### 3.5.3 Maintainability
Specify attributes of software that relate to the ease of maintenance of the software itself. These may include requirements for certain modularity, interfaces, or complexity limitation. Requirements should not be placed here just because they are thought to be good design practices.

#### 3.5.4 Reusability
<!-- TODO: come up with a description -->

#### 3.5.5 Portability
Specify attributes of software that relate to the ease of porting the software to other host machines and/or operating systems.

#### 3.5.6 Cost
Specify monetary cost of the software product.

#### 3.5.7 Deadline
Specify schedule for delivery of the software product.

#### 3.5.8 Proof of Concept
<!-- TODO: come up with a description -->

## 4. Verification
> This section provides the verification approaches and methods planned to qualify the software. The information items for verification are recommended to be given in a parallel manner with the requirement items in Section 3. The purpose of the verification process is to provide objective evidence that a system or system element fulfills its specified requirements and characteristics.

<!-- TODO: give more guidance, similar to section 3 -->
<!-- ieee 15288:2015 -->

## 5. Appendixes
