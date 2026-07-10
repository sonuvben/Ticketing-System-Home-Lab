**IT Service Desk & Ticketing System Home Lab**  
A hands-on project exploring enterprise IT service management and incident reslution. I built this environment to tackle the daily operations of a helpdesk professional: ticket triage, SLA management, knowledge base integration, and resolving infrastructure issues.

**Why I Built This**  
This project was built to develop practical, demonstrable ITSM skills for entry-level helpdesk roles.

**Overview**  
I deployed and configured Jira Service Management (JSM) as an enterprise ticketing system, integrating it directly with my existing Windows Server 2022 Active Directory lab. The project involves setting up request categories, defining Service Level Agreements (SLAs), automating ticket routing, configuring ticket priority levels, and integrating a Confluence knowledge base. To cover the core tasks of a helpdesk role, I executed a full simulation by generating and resolving tickets for account lockouts, user provisioning, and DNS connectivity issues using actions within AD DS.

**Tech Stack**  
- Jira Service Management (JSM)
- Confluence (Knowledge Base)
- Windows Server 2022 (Active Directory Users and Computers)
- Windows 11 Enterprise
- PowerShell/Command Prompt

**Architecture & Environment**  
- Ticketing Platform: Jira Service Management configured with four major request categories: Incident, Service, Access, and General Support.
- SLA Configuration: Time to First Response and Time to Resolution clocks tied to standard 9-5 business hours; Time to Close operates on a 24/7 calendar.
- Priority Matrix: Structured priority queue scheme handling P1 (critical) through P4 (low) incidents.
- Backend Infrastructure: Integrated with an on-premise 192.168.15.0/24 Windows domain network for live ticket resolution and client troubleshooting.

**Build Log** 
Day-by-day record of the entire build process, including challenges encountered and solutions used.

**Key Learnings** 
- Platform Administration & Triage: Gained hands-on experience configuring an enterprise service desk, translating high-volume prioritization skills into structured IT workflows using P1-P4 priority schemes and ordered queues.
- Active Directory Integration: Bridged the gap between ticketing and infrastructure by executing real administrative tasks—such as user provisioning, security group assignments, and password resets—in response to simulated user requests.
- Workflow Automation: Learned how to track and manage response metrics by configuring custom SLA calendars and building automation rules for ticket assignment and threshold warnings.
- Knowledge Management: Demonstrated the value of centralized documentation by writing and linking Confluence KB articles, streamlining the troubleshooting process for internal agents.
- Diagnostic Methodologies: Applied structured troubleshooting steps to diagnose client-to-server connectivity, isolating network faults using standard command-line utilities and documenting the resolutions as reproducible runbooks.

**Next Steps**  
I plan to implement a ServiceNow version of this project to compare popular ITSM implementations. I will also utilize the diagnostic methodologies and troubleshooting practiced in this lab to prepare for the CompTIA A+ certification exams.


  
