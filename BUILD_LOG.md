**Build Log** 

July 3: ServiceNow 
- Created a ServiceNow account and requested a Private Developer Instance. I'm waiting to get off their waitlist. 
  
July 8: Platform Configuration and SLAs  
- The demand for ServiceNow PDIs are just too high, so I set up a Jira Service Management environment instead.  Created the four primary request categories and established the P1-P4 priority scheme. Defined custom SLA metrics for Time to First Response, Time to Resolution, and Time to Close after resolution. Configured the calendars so the resolution timers strictly tick during standard 9-5 business hours, while the closure timer utilizes a 24/7 schedule.

July 9: Queues, Automation, and Knowledge Base  
- Implemented three dedicated agent views: a priority queue, an SLA queue, and a general view queue. Designed automation rules to handle automatic ticket assignment and trigger SLA threshold warnings. Signed up for Confluence, authored a knowledge base article on troubleshooting network drives, and linked the space directly to JSM.
  - **Challenge/Solution:** The Confluence free tier doesn't grant external visibility for linked knowledge base articles. Copied and uploaded the KB article to this repo as a raw text file instead.

July 10: Active Directory Administration & Helpdesk Ticket Resolution  
- User Provisioning & Group Policy Management: Executed an end-to-end onboarding workflow for a new hire. Provisioned the account via Active Directory Users and Computers (ADUC) and enforced an initial password reset upon first logon for security compliance. Assigned the user to the Finance Security Group, ensuring role-based access control and the successful application of departmental Group Policy Objects (GPOs) for secure folder access.
  
- Account Security & Identity Management: Processed a simulated Priority 2 (P2) account lockout incident. Diagnosed the lockout status within ADUC, cleared the flag, and issued a secure password reset. Maintained clear, professional communication with the end-user via Jira Service Management ticket comments and documented the root cause before closing the request.
  
- Network Diagnostics & PowerShell Administration: Resolved a simulated DNS failure on a client machine. Applied a structured diagnostic methodology, using ping to test local broadcast connectivity and nslookup to definitively isolate the failure to the DNS layer. Bypassed user-level GUI restrictions by deploying an elevated PowerShell command (Set-DnsClientServerAddress -ResetServerAddresses) to restore DHCP configurations and resolve the ticket within the established SLA threshold.
  - **Challenge/Solution:** While diagnosing the inaccessible network drive, I used ping on the DC/DNS/DHCP servers and it successfully went through. This was surprising because I had deliebrately broken the DNS connection. After some review, I realized that Windows uses protocols like NetBios to resolve pings through broadcasts. So instead, I used nslookup localhost to isolate the DNS as the issue. 

