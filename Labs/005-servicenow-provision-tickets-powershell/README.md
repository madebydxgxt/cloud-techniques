# servicenow-ticket-provisioning-powershell

A hands-on lab demonstrating how to provision (create) ServiceNow incident tickets by sending a REST API payload from a PowerShell script.

## Watch me build this lab
https://www.loom.com/share/3279ef8336d54e54b0492462505d576d

**What this video shows:** Running a PowerShell script that posts an incident payload to a ServiceNow developer instance and then verifying the created ticket inside the Incident list.

---

## Objective
Automate the creation of ServiceNow incident tickets by pushing data to a ServiceNow instance using a PowerShell script.

---

## Skills Practiced
- PowerShell scripting for automation
- Working with a ServiceNow Developer Instance
- Calling REST APIs from PowerShell (Invoke-RestMethod)
- Basic authentication / credential handling (high-level)
- Building and sending a request payload (example: JSON body)
- Interpreting API responses (success flags + returned identifiers)
- Verifying records in ServiceNow (Incident table search)
- Basic troubleshooting when records don’t immediately appear

---

## Tools Used
- ServiceNow Developer Instance
- ServiceNow Incident table/module
- Windows PowerShell (PowerShell terminal)
- ServiceNow REST/Table API (example: Incident endpoint)
- (Optional) Text editor or IDE for script review (example: VS Code)

---

## Steps Performed
1. **Set up a ServiceNow developer instance**  
   Identified the ServiceNow instance URL and gathered the basic account credentials needed to authenticate API requests.  
   (Optional screenshot) docs/step-1.png

2. **Review and customize the PowerShell script**  
   Updated the script with the instance details and user credentials, and confirmed the request payload fields were set for ticket creation.  
   (Optional screenshot) docs/step-2.png

3. **Prepare the API request payload**  
   Defined a simple ticket payload (example: short description and other common fields) to send to ServiceNow via the API.  
   (Optional screenshot) docs/step-3.png

4. **Execute the script to create a ticket**  
   Ran the PowerShell script to post the payload to ServiceNow and create a new incident record.  
   (Optional screenshot) docs/step-4.png

5. **Capture the created ticket identifier from the response**  
   Checked the output for the returned incident identifier/number (example shown in the video: `task_effective_number`) to use for lookup.  
   (Optional screenshot) docs/step-5.png

6. **Verify the incident in ServiceNow**  
   Opened the Incident list in ServiceNow and searched for the returned ticket number to confirm the record was created successfully.  
   (Optional screenshot) docs/step-6.png

7. **Troubleshoot record visibility (if needed)**  
   Refreshed and re-checked the Incident list/search when the ticket did not appear immediately, then confirmed it was present.  
   (Optional screenshot) docs/step-7.png

---

## Outcome
Successfully created a ServiceNow incident via a PowerShell REST call and confirmed the new ticket appeared in the ServiceNow Incident list.
