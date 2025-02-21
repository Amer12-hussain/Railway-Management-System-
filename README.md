This project manages train reservations using classes and arrays for structured data handling.

Classes & Data Members:
TrainClass:

cid: Unique class ID (int)
cname: Class name (string)
Train:

tid: Unique train ID (int)
cname: Train name (string)
source: Starting station (string)
destination: Ending station (string)
TrainCapacity:

cid: Valid if exists in TrainClass
tid: Valid if exists in Train
totalSeats: Total seats (int)
rate: Fare rate (int)
Reservations:

cid, tid: Valid if exists in TrainCapacity
date: Format dd/mm/yyyy
ticketNo: Auto-generated based on available seats
CNIC: Passenger's ID (string)
passengerName: Alphabets only (string)
Operations:
TrainClass: Insert, update (cname), delete (if unused), display all or by cid
Train: Insert, update (cname), delete (if unused), display all or by tid
TrainCapacity: Insert, update (attributes except tid+cid), delete (if unused), display all or by tid+cid
Reservations: Insert, update (excluding tid+cid+ticketNo+date), delete, display all, display by tid+cid+date, show available seats
