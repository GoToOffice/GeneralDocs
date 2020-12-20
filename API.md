# APIs list:

## User

updateUser(user:User) <sub>(Orly, Oz)</sub>  
deleteUser(user:User) <sub>(Orly, Oz)</sub>  
User getUser(userId:String) <sub>(Orly, Oz)</sub>   

```diff
- we don't need this, get the user and check: Boolean isAdminUser()
```

```json
User 
{
  "id": "1234",
  "name": "myName",
  "displayName": "myDisplayName",
  "isAdmin": false,
  "email": "email@gmail.com",
  "profilePicture": ""
}
```



## Office

createOffice(office:Office) <sub>(Orly)</sub>  
deleteOffice(office:Office) <sub>(Orly)</sub>   
updateOffice(officeId:String) <sub>(Orly)</sub>   
List<Office> getOffices() <sub>(Orly, Omer)</sub>  
Office getOffice(officeId:String) <sub>(Orly)</sub>  

```json
Office:
{
  "id":"326587243653",
  "name":"myOffice",
  "description":"Best office",
  "country": "..."
}
```


## Seat

addSeat(officeId:String, seat:Seat) <sub>(Orly)</sub>  
deleteSeat(officeId:String, seatId:String) <sub>(Orly)</sub>  
updateSeat(officeId:String, seatId:String) <sub>(Orly)</sub>  
List<Seat> getSeats(officeId:String) <sub>(Orly)</sub>  
Seat getSeat(officeId:String, seatId:String) <sub>(Orly)</sub>  
List<Seat> getListOfAvailableSeats(officeId:String, startTime:String, endTime:String) <sub>(Omer)</sub>  

```json
Seat:
{
  "id":"1588263592921",
  "type" : "FullyEquip",
  "chairType" : "Adjustable",
  "location" : "next to a window",
  "roomId" : "1588263592911",
  "officeId": "82746283746"
}
```


