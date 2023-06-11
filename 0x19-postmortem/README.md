# Postmortem

During the development of a project called a school management system using the Odoo framework. I have faced an outage and here is a summary of that outage.

### Issue Summary

* Duration of the outage: The outage occurred on 8 June from 2pm to 6pm East Africa Time (EAT, GMT+3).
* Impact: The lack of a security file caused an access rights issue, resulting in a service disruption. I have experienced restricted access or inability to perform certain actions during the outage. It affected 100% of the system during that time.
* Root Cause: The root cause of the issue was the absence of a security file that defined the access rights, leading to unauthorized access restrictions within the system.

### Timeline

* Issue detection: The issue was detected at 2pm on 8 June (EAT) when the developer experienced restricted access and permission errors while testing the system.
* Detection method: The developer noticed the issue while interacting with the system during the testing phase.
* Actions taken: The developer investigated different parts of the system, including the access control mechanisms and user permission settings. Initially, the assumption was that the issue might be related to recent updates in the system's authentication module.
* Misleading investigation paths: The developer initially focused on the authentication module and spent time debugging the related code, assuming that recent changes might have caused the problem. However, this path did not lead to the root cause.
* Escalation: As the incident persisted, the developer sought assistance from senior team members and the system administrator for further analysis and resolution.
* Incident resolution: After thorough investigation, it was discovered that the absence of a security file was causing the access rights issue. The security file was promptly created, defining the necessary access permissions for different user roles, and deployed to the system. This resolved the access rights problem, restoring normal functionality.
Root Cause and Resolution
The root cause of the issue was identified as the lack of a security file that defined the access rights within the system. Without this file, the system was unable to properly authenticate and authorize users, leading to restricted access or permission errors. To fix the issue, the developer created the necessary security file, specifying the access rights for each user role. Once the file was added to the system, access restrictions were lifted, allowing the developer to perform intended actions.

### Corrective and Preventative Measures
To prevent similar issues in the future, the following corrective and preventative measures will be implemented:
* Improve the system's security architecture by ensuring that access rights are properly defined and enforced through robust mechanisms.
* Implement regular security audits and checks to identify any missing or misconfigured security components.
* Establish a thorough testing process to verify the functionality and access rights of different user roles.
* Develop and enforce a standard procedure for creating and maintaining security files, ensuring they are included in all relevant deployments.
* Provide training and guidelines for developers to emphasize the importance of access control and security measures.
* Add automated monitoring systems to detect access rights discrepancies or configuration errors.

## Tasks to address the issue
* Create and deploy the security file defining access rights.
* Perform a comprehensive review of the system's security architecture.
* Develop a testing plan to verify access rights for different user roles.
* Establish a procedure for maintaining and updating security files.
* Implement automated monitoring systems to detect access rights issues.

