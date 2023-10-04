---
title: "Day 14 Exercise 1"
weight: 5
---

### Instructors Chaos List: Chaos Selection
In this activity, you and the TA's are part of the Security Analyst team. One of you will pull an item from the Chaos List and allow one member from the team to come up in front of the class and read the problem and responsible teams. One team at a time is selected to read aloud and to reveal the disruption. Each team is responsible for implementing the new business strategy for the problem. Allow the team 10 minutes to address the disruption as creatively and effectively as possible. Each situation includes the story points required to complete the task. These points are used to reduce employee burnout. Each team has a maximum of 25 Story points. Any points above this have a negative impact on performance and quality. For task greater than 10 points you can assign multiple members to work on the task using a collaboration tool like Google Docs or Microsoft Word. You can introduce items for both list at the same time or at different times it's your class. Have fun!  

## Material: 
**Index Cards**
Give each group 10-15 index cards. When a chaos situation is introduced, use the index card to capture the change

**Chaos Business Rules of engagement** 
The Chaos Business Rules can only be introduced by the instructor and should be selected at random. These rules do not need to come from this list and can be created by ad hoc by the instructor. The time associated with Low priority task is also selected at random by the instructor. 

Every 5 minutes, the instructor should pull an item form the list Development, Operation and Approval Team and have a member from the team come up an introduce the Chaos. The responsible teams have to work on a solution for 10m then start the approval process to ensure they've checked all the boxes. 

**High Priority (@20m each)**
1. With the rise of security concerns and Ransomware we need a backup and recovery strategy (10pts).
2. Security compliance with PII (20pts) - Impacts all teams 
3. Legal compliance archive strategy (20pts) - Impacts all teams 
4. Remove 1 team member at random (0pts)
5. Switch a team member to another team (0pts) 

**Low Priority (@1-15m each)**
1. Load Balancer (4pts) - Impacts Development and Operations 
2. Databases backed up? (5pts) - Impacts Development and Operations 
3. Redundancy and fault tolerance (15pts) - Impacts Development and Operations 
4. Application has a capacity plan? (10pts) - Impacts Development and Operations 
5. Has the operations team been notified and have reviewed the project? (5pts). 
6. Applications must be fault tolerant? (10pts) - Impacts Development and Operations 
7. Application have to be cloud native? (8pts) - Impacts Development and Operations 

# Development Team (Chaos List)
1. Production Webserver not responding (7pts) 
2. Database slow response rate (5pts) 
3. Page-load slow performance (5pts)
4. Security Vulnerabilities in software (20pts) 
5. PII data lead (10pts)

# Operations Team (Chaos List)
1. Is there a test plan? 
2. How many severs are needed? 
3. Is there a capacity plan? 
4. Is there a business continuity (BC) or disaster recovery plan (DR)? 
5. Does the application have redundancy or fault tolerance 

# Approval Team (Chaos List)
1. Is this new business account or existing account - All Teams
2. What is the Market size - Business Team 
3. Does the product have a customer persona - Business Team 
4. Are there any key relationships needed for the business to reach its goals
5. Does this product have an MVP? 
6. Is there a QA Plan? 

## Instructor Notes:
Once the activity ends discuss that in a real world situations the teams would have months to apply changes and have legal and compliance teams that will having conversations at higher levels of the organization before they become concerns for the enterprise. Also, highlight that some changes are faster than others and will have a more immediate impact like what was introduced in this simulated environment. If the development team builds a Web application, ask them why? There should have been a red flag when the QR code and permissions for camera access. 

## Customer Team 
Responsibilities 
- Product Owner 
- Only communicates with the Business Team

Customer Request
Create a website that allows us to capture client emails and name during a conference event. The application should allow QR code scanner that allows clients to scan our the QR code and show the contact details of the person they are meeting with. We'd like an API that allows third-party teams to query events that they've attended. 

Application Requirements 
1. **QR Code Scanner:**
   - Access to the device's camera for scanning QR codes.
   - Integration with a QR code scanning library or API.

2. **User Authentication:**
   - If your app involves user-specific data or actions, implement a secure authentication system.

3. **Data Processing:**
   - Ability to interpret and process data encoded in QR codes.
   - Handle various QR code formats (URLs, text, contact information, etc.).

4. **Database:**
   - Store and retrieve relevant data associated with scanned QR codes.

5. **User Interface:**
   - Intuitive design for the scanner interface.
   - Clear feedback on successful scans or errors.

6. **Permissions:**
   - Request necessary permissions, such as camera access.

7. **Offline Support:**
   - Consider functionality for situations where the device may not have an internet connection.

8. **Error Handling:**
   - Robust error handling for scenarios like invalid QR codes or camera issues.

9. **Security:**
   - Implement secure coding practices to protect user data.
   - Ensure that scanned QR codes don't pose security risks.

10. **Customization:**
    - Allow users to customize their experience, such as choosing default actions for specific QR code types.

11. **Integration with Other Services:**
    - If applicable, integrate with other services or APIs based on the scanned QR code data.

12. **Analytics:**
    - Implement analytics to track user engagement, popular QR codes, etc.

13. **Platform Compatibility:**
    - Develop the app for the platforms you want to support (iOS, Android, etc.).

14. **Testing:**
    - Thoroughly test the app for various scenarios, devices, and edge cases.

15. **Documentation:**
    - Provide documentation for users and developers, explaining how to use the app and any APIs it exposes.

16. **Compliance:**
    - Ensure compliance with relevant data protection and privacy regulations.

## Approval Team 
The approval team is always busy and it take 2 minutes to approve everything in this simulated environment. They also have a 5-item limit before they can take new approvals. All approvals after 5 have hit their queue and be placed on hold. If they are working on a high priority item, no new request can be taken.  If a team does not have all the required items for the approval, they are sent back to the responsible team to collect the item required. 

**Only communicates with the Business Team** 

Checklist 
New business account 
1. Meet our current organizational goals 
2. Create new revenue?  
3. Create new customers?
4. Expand our existing customer base?  
5. Create product awareness or is it a new product? 

## Operations Team (required)
Responsibilities
- Ensure all Approvals have been met before deployment to production environments 
- Application security 
- Only communicates with the Development Team
- Request an update from the Business Team on the application 

**Checklist** 
1. Is there a test plan? 
2. How many severs are needed? 
3. Is there a capacity plan? 
4. Is there a business continuity (BC) or disaster recovery plan (DR)? 
5. Does the application have redundancy? fault tolerance 

## Business Team 
Business Team 
Primary responsibilities is meeting with the Customer Team and gathering requirements for the development team. 
Responsibilities 
- Communicates to the Technical team what they are doing and when it is done.
- Connect the Developers with the Business Analysis and customer needs 
- Only communicates with the Customer Team & Project Manager
    
The business analysis will meet with the customer to discuss a web or mobile application and the features required for the application. The customer can request both a mobile app and web application. Once the requirements are collected and the features have been defined, the Business Analyst will meet with the development team to discuss the features and the Development team will create a 

1. Project timeline 
2. Project roadmap
3. System architecture and 
4. Dataflow diagram 

Once these 3 documents are created and approved by the Project Manager they will be presented to the customer for review and approval. Once they have been approved by the customer, they documents will be sent to the Approval Team for review and approval/rejection to ensure the work aligns with the business needs. 

## Development Team  
This team consist of 1 Project Manager, 1 or more web developer(s), 1 or more mobile app developer(s). Developers have a 10-story point limit. Once this limit is maxed the projects will incur a wait time of 15m before they can be started or introduced to the development team. Project marked with high critical levels you must have developers stop what they are doing and begin working on them immediately. 

## Reflection group Questions 
1. What went well? 
   1. What would you do differently? 
2. How did you feel? 
3. How was the pace? 
4. How would effective communcations help? 
 


