We built a system that track and compute cars entry & exit from parking lots, as well as compute their charge. 
The system is based on a serverless solution. 

Download the attached zip file and run the setup.sh script.
Two URL will be printed for the two HTTP endpoints: 
•	ENDPOINT ENTRY
•	ENDPOINT EXIT

For entry endpoint run:
ENDPOINT_ENTRY_URL/entry?plate=<plate_number>&parkingLot=<parking_lot_number>
For example: ENDPOINT_ENTRY_URL/entry?plate=123-123-123&parkingLot=382 
Returns the ticketId.
For exit endpoint run:

EXIT_ENTRY_URL/exit?ticketId=<ticket-id>
For example: EXIT_ENTRY_URL/exit?ticketId=1234
Returns the license plate, total parked time, the parking lot id and the charge (based on 15 minutes increments).
