# Vacation-tracking-system
# Manage time use case
#Flow chart
<img width="2091" height="486" alt="chart drawio" src="https://github.com/user-attachments/assets/1f8c9f6e-5439-4182-8299-2fbaed432d0b" />

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
