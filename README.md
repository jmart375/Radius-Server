# Security Requrirements
# Table of Contents
1. [Step 1: Build, install and configure the RADIUS Server](#step-1-build-install-and-configure-the-radius-server)
2. [Step 2. Build access control policy](#step-2-build-access-control-policy)
   - [DETERMINE TEAMMATES TO BUILD ACCESS CONTROL POLICY](#determine-teammates-to-build-access-control-policy)
   - [ACCESS CONTROL](#access-control)
   - [CONTROL PURPOSE](#control-purpose)
   - [POLICY](#policy)
3. [Step 3. Model (Architect) the access control policy](#step-3-model-architect-the-access-control-policy)
4. [Step 4. Test Plan](#step-4-test-plan)
   - [INTRODUCTION](#introduction)
   - [TESTABILITY](#testability)
   - [THE TEST PROCESS: THE PLAN, TEST SPECIFICATIONS, AND TEST RESULTS](#the-test-process-the-plan-test-specifications-and-test-results)
      - [Test report](#test-report)
      - [Test Planning](#test-planning)
      - [Checking results](#checking-results)
   - [SOFTWARE REQUIREMENTS](#software-requirements)
   - [TEST OUTPUT FIELDS](#test-output-fields)
   - [PROJECT FUNCTIONS](#project-functions)
      - [PROJECT IDENTIFICATION](#project-identification)
      - [Program Manager](#program-manager)
      - [Project Manager](#project-manager)
      - [Test Manager](#test-manager)
      - [Test Lead](#test-lead)
      - [TESTING TYPES](#testing-types)
5. [VERIFICATION](#verification)

## Step 1: Build, install and configure the RADIUS Server.
[Details on building, installing, and configuring the RADIUS Server]
![image](https://github.com/jmart375/Radius-Server/assets/91294710/b1bcdba1-e37e-49ad-bb0f-a8e40e4321ff)

Policy Showing Guest Access is restricted to users that are not in the “VPN” Group.
![image](https://github.com/jmart375/Radius-Server/assets/91294710/f23f3e15-185a-4118-b997-31ff25665683)

Access Granted to “Fatima” as she is an Approved User and has the required Roles.
![image](https://github.com/jmart375/Radius-Server/assets/91294710/fc404a0c-f1f9-49d1-bf8b-9d1325b6a38d)

5 Roles were created to separate the diverse types and connections that are allowed on the VPN.
![image](https://github.com/jmart375/Radius-Server/assets/91294710/8fe579e9-0226-4f86-b854-08771fb2e26a)

Different Objects with multiple controls to within the objects to limit/grant access.
![image](https://github.com/jmart375/Radius-Server/assets/91294710/107dd4f9-5116-4917-9e5c-2fb00e3e62f1)

Verifying we do not allow Guest, with membership to the group “Guest” on to the VPN.
![image](https://github.com/jmart375/Radius-Server/assets/91294710/8a4999c5-0a93-4c8d-9376-7660c81c52ef)

Selected “No Guests...” you can see multiple objects configured to prevent access at multiple levels.
![image](https://github.com/jmart375/Radius-Server/assets/91294710/55ba9974-fcb3-45cf-9709-6537ef1ed8ee)

Roles are user and group-based access controls.

## Step 2. Build access control policy
1. **DETERMINE TEAMMATES TO BUILD ACCESS CONTROL POLICY**
   - With the proper application controls, businesses and organizations greatly reduce the risks and threats associated with application usage because applications are prevented from executing if they put the network or sensitive data at risk.
   - Why is access control important? The goal of access control is to minimize the security risk of unauthorized access to physical and logical systems.
   - Who decides how and when data in an organization will be used or controlled? Control and use of data in the Data owners are responsible for how and when data will be used, Data users are working with the data in their daily jobs.

2. **ACCESS CONTROL**
   - The rapid transformation to the digital world has required major changes to how organizations manage their workforce and in particular how they deliver and govern access to critical applications and data.
   - That workforce is no longer just human users; employees, contractors and vendors, but also bots or service accounts each needing their own set of access requirements, restrictions, and locations. Additionally, data and applications spread cross cloud, on premises and hybrid infrastructures are being accessed from anywhere, on a variety of devices. Today many organizations are relying on identity tools designed to quickly authenticate and federate access to workers. While these tools offer basic lifecycle management capabilities to enable workers with 24/7 access, they lack the needed security access controls and policies required to effectively know who can access what and more importantly deliver access based on who can access what and more importantly deliver access based on who should access what. 

3. **CONTROL PURPOSE**
   - An access control policy provides rules and guidelines structuring who can access data and resources at an organization. It takes the form of a document offering a high-level overview and is then implemented via more specific rules and procedures.

4. **POLICY**
   1) **Account Management**
      - Identify and select the following types of information system accounts...
   2) **Access Enforcement**
      - Ensure that the information system enforces approved authorizations...
   3) **Information Flow Enforcement**
      - Ensure that the information system enforces approved authorizations...
   4) **Separation of Duties**
      - Separate duties of individuals as necessary, to prevent malevolent activity without collusion...
   5) **Least Privilege**
      - Employ the principle of least privilege...
   6) **Unsuccessful Logon Attempts**
      - Enforces a limit of consecutive invalid logon attempts...
   7) **System Use Notification**
      - Displays to users an approved system use notification message...
   8) **Session Lock**
      - Prevent further access to the system by initiating a session lock...
   9) **Session Termination**
      - Ensure that the information system automatically terminates a user session...

5. **COMPLIANCE**
   - Employees who violate this policy may be subject to appropriate disciplinary action up to and including discharge as well as both civil and criminal penalties. Non-employees, including, without limitation, contractors, may be subject to termination of contractual agreements, denial of access to IT resources, and other actions as well as both civil and criminal penalties.

## Step 3. Model (Architect) the access control policy
[Details on modeling/architecting the access control policy]
![image](https://github.com/jmart375/Radius-Server/assets/91294710/6a67e3c2-93ff-468e-b2c6-45230cad2ee1)

## Step 4. Test Plan
1. **INTRODUCTION**
   - This document is intended to outline the Radius Server Lab test strategy and overall test approach. This includes test methodologies, implementations, and specifications.
   - The goal is to provide a working Radius Server on the virtualized network. As well as demonstrate framework that can be used by organizations and testers to plan and execute the necessary tests in a timely and cost-effective manner.

2. **TESTABILITY**
   - The Radius test is aimed to demonstrate the operations of the Radius Server...


3. **THE TEST PROCESS: THE PLAN, TEST SPECIFICATIONS, AND TEST RESULTS**
   1. **Test report**
      - The test cases must be executed, and results must be reported...
   2. **Test Planning**
      - The goals of test planning are to coordinate certain tests and make relevant decisions...
   3. **Checking results**
      - After test planning has been conducted, you will follow by checking the results...
   - Acceptance Testing
      - The final stage before taking the system into full operation is to let the customers and users check that the system fulfills their actual needs.

4. **SOFTWARE REQUIREMENTS**
   - The hardware components in the system are a Database Server, a Webserver, a client PC with a web browser.

5. **TEST OUTPUT FIELDS**
   | Field Name            | Field Description                                                                                           |
   |-----------------------|-------------------------------------------------------------------------------------------------------------|
   | Server                | The IP address of the Radius server authenticated                                                             |
   | UDP port              | The Radius server port utilized during the authentication test                                                |
   | Source IP Address     | “Default” is shown if the IP address is the same as that of the Radius server.                                |
   | Server Timeout        | The Radius server timeout period.                                                                             |
   | Server retry count    | The number of authentication attempts allowed by the Radius server.                                            |
   | Secret                | The shared secret used for authentication with the Radius server.                                              |
   | Client Username       | The username authenticated by the Radius server.                                                              |
   | Client Password       | The user password authenticated by the Radius server                                                          |
   | Status                | The test result status (Accepted or Rejected) and the number of retransmits utilized during authentication.  |
![image](https://github.com/jmart375/Radius-Server/assets/91294710/2ce389d3-8b06-45c4-abe1-3e45e7a7fa7d)

   - Output example 1

6. **PROJECT FUNCTIONS**
   - **PROJECT IDENTIFICATION**
      | Project Name | Project Number | Date Created |
      |--------------|----------------|--------------|
      | Radius Server | 3              | 6/22/22      |

   - **Program Manager**
   - **Project Manager**
   - **Test Manager**
   - **Test Lead**
![image](https://github.com/jmart375/Radius-Server/assets/91294710/dc0c0731-f0bf-4068-91ed-b540ad16f92f)

   6.1 **TESTING TYPES**
   | Type of Test                 | Will Test Be Performed? | Comments/Explanations | Pass / Fail |
   |------------------------------|-------------------------|------------------------|-------------|
   | Does VPN connect             | Yes                     | No                     |             |
   | Are user groups enforced      | Yes                     | No                     |
