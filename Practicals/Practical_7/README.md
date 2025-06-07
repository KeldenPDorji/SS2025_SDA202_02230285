# Car Management System - Sequence Diagrams  

## **Core Flows**  

### **1. Car Rental Process**  
- Desk Officer enters car details  
- System validates & finds car  
- Car details displayed → can be modified  
- On success:  
  - Car marked as "rented"  
  - Payment processed  
  - Success confirmation shown  

### **2. Car Update Process**  
- Desk Officer provides car plate number  
- System retrieves & displays car info  
- Officer submits updates  
- System confirms successful update  

## **Participants**  
- **Forms**: Rental (FormRentCar) & Update (FormUpdateCar) interfaces  
- **Controllers**: RentCarController & UpdateCarControl logic handlers  
- **Car**: Maintains vehicle data/status  
- **BillingSystem**: Processes payments  

## **Visualization**  
1. Use any PlantUML renderer  
2. Paste the provided diagram code  
3. Generate to view interaction flows  

> Tip: The diagram separates rental and update logic while sharing the Car resource