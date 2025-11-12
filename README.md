# Vacation-tracking-system
* Vision 

  A Vacation Tracking System (VTS) will provide individual employees with the capability to manage their own vacation time, sick leave, and personal time off, without having to be an expert in company policy or the local     facility’s leave policies.

* Function Req
    - Employee must be able to check his own balance.
    - Enables manager approval (optional).
    - Implements a flexible rules-based system for validating and verifying leave time requests.
    - Provides access to requests for the previous calendar year, and allows requests to be made up to a year and a half in the future.
    - Uses e-mail notification to request manager approval and notify employees of request status changes.

* Non‑Functional Req
  - The system must be easy to use.
  - Uses existing hardware and middleware.

* Constraints
  - Integration between portal with all leagacy data and roles and the new VTS.
  - it must be friendly to use for non-technical (HR)

* Actors
  - Employee
  - Manager
  - HR
  - Admin
    
  
# Manage time use case
#Flow chart
<img width="2091" height="486" alt="manageTimeFlowChart" src="https://github.com/user-attachments/assets/ccc985b2-3b08-46d1-81be-107a7005e775" />


#Sequence Diagram
<img width="1151" height="1571" alt="vtsSequenceDiagram drawio" src="https://github.com/user-attachments/assets/fe479eb7-9adb-46e2-803b-98c0406f87fe" />

#Pseudocode 

signInPortal()
If employee is authenticated in portal, employee can login VTS and check his balance of vacations.
Else return invalid credentials.

SubmitVacationRequest(vacationCatalog, date)
Validate the request according to the info submitted by the employee.
If validation failed, return the error and the employee has the ability to modify info.
Else If it require manager approval -> return status is pending and send an email to the manager.
Else Vacation granted if it don't require the manager approval.

signInPortal()
If manager is authenticated in portal, manager can login VTS and check his pending list with all info related to the requests.
Else return invalid credentials.

VacationResponse()
If the manager grant the vacation, an email will be sent to the employee with the approval.
Else the manager will state the reasons why he rejected the vacation request and it will be sent to the employee.

# Withdraw Request use case
#Flow chart

<img width="380" height="891" alt="flowChart drawio" src="https://github.com/user-attachments/assets/fb17f7a8-b754-4ceb-a3f0-bf993765c364" />

#Sequence diagram

<img width="931" height="931" alt="withDrawSequenceDiagram drawio" src="https://github.com/user-attachments/assets/c126aad7-6180-4090-a225-4845e061fddb" />

# Cancel approved Request use case
#Flow chart



#Sequence chart
<img width="911" height="1041" alt="cancelApprovedSequenceDiagram drawio" src="https://github.com/user-attachments/assets/53d02664-8efe-4379-9144-b3498f5666d0" />

# Edit a vacation request use case
#Flow chart

<img width="541" height="1141" alt="editPendingRequest drawio" src="https://github.com/user-attachments/assets/cc4390ae-fa0a-4103-99b8-d890b4373fe0" />

#Sequence chart

<img width="771" height="1011" alt="editRequestSequenceChart drawio" src="https://github.com/user-attachments/assets/886f8123-2b2d-44b6-a57d-467162bbbac0" />


# ERD Diagram

<img width="749" height="1242" alt="ERD drawio" src="https://github.com/user-attachments/assets/71f81543-10c3-447f-b033-544bbb07f45f" />
