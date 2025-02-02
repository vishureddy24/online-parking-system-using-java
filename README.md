# online-parking-system-using-java
Parking System - Project Description

Introduction

The parking system is an easy, though efficient, console application built on Java, whose purpose is the management of available parking places within a controlled environment. It can park cars, remove parked cars, and shows currently parked vehicles** using an easy-to-understand menu-driven interface.

A very common issue that arises while dealing with an urban area, shopping malls, office buildings, or residential complex is the management of parking space. This parking management system enables the easy operation of the facility in such a manner that available spaces are effectively utilized, the place is devoid of congestion, and the customer is satisfied.

---

Project Objectives

The key objectives for the Parking System project are:

1. A simple and efficient method to dynamically manage parking slots.
2. Allow users to park and retrieve their cars with just a license plate number. 3. TO track available slots so that a user cannot park if there are no available slots. 4. Provide an easy, interactive way to see all the cars parked in the system. 

---

Features and Functionalities 

1. Dynamic Slot Management
- The total number of available parking slots in the system may be defined during initialization. 
   - This number is modified as cars get parked and as they leave, updating the availability of slots in the system.

2. Parking a Car 
   - License plate number may be input into the system in order to park a car.
- The system checks if a parking slot is available before parking.  
   - If parking slots are full, a message informs the user that no spaces are available.  

3. Remove a Car  
   - Users can remove a parked car by entering its license plate number.
- The system first checks if the car is parked before allowing its removal.  
   - The number of available slots increases when a car is removed.  


4. View Parked Cars  
   - Users can view all cars currently parked in the system.  
   - In case no car is parked, an appropriate message is displayed.

5. Menu-Driven Interface for User Action Selection
   The system provides a menu-driven interface to the user for selecting the action. 
   The options are parking a car, removing a car, viewing parked cars, or exiting the system. 

---

Implementation Details

1. Programming Language: Java
2. Data Structure Used: `ArrayList<String>` (to store parked cars)
3. Input/Output Handling:
- Scanner is used to take user inputs dynamically.  
   - Print statements are used to guide users and display relevant messages.  
4. Loop Structure:  
   - The system runs in an infinite loop (`while(true)`) until the user chooses to exit.  
   - A `switch-case` statement is used for user interaction.  

---

Code Breakdown

1. Initialization  - The system first asks the user to input the total number of parking slots.  - The number of available slots is initialized according to this input. 

2. User Interaction (Main Menu)  - The system continues to display the menu until the user decides to quit.
-Users can pick selections by numbering (1 for parking, 2 for removal, and so on).
 
3. Parking of a Car (`parkCar()` Method) 
   -When a parking slot is available, ask the user to input the license plate number of the car
   -Store the license plate in the `ArrayList` and decrement the count for slots available.

4. Remove a Car (`removeCar()` Method)  - The system prompts the user to input the license plate number of the car to be removed.  - If the car is located in the list, it is removed and available slots are incremented. 

5. View Parked Cars (`viewParkedCars()` Method)  - The system shows all parked cars if any exist.
- If there is no parked cars, the output message appears right.

Example Run


Enter the total number of parking slots:
5

What would you like to do?
1. Park a car
2. Remove a car
3. View parked cars
4. Exit
Choice: 1

Enter the license plate number of the car:
ABC-123

Car parked successfully. Available slots: 4

What would you like to do?
1. Park a car
2. Remove a car
3. View parked cars
4. Exit
Choice: 3

Parked cars:
ABC-123

What would you like to do?
1. Park a car
2. Remove a car
3. View parked cars
4. Exit
Choice: 2

Enter the license plate number of the car to be removed:
ABC-123
Car removed successfully. Available slots: 5

Parking System - Project Description
The Parking System is a simple, efficient Java-based console application for the management of parking spaces in a controlled environment. This system enables users to park cars, remove parked cars, and view currently parked vehicles** with a user-friendly menu-driven interface.

Managing parking spaces effectively is a common challenge in urban areas, shopping malls, office buildings, and residential complexes. This project provides an easy-to-use parking management system that ensures efficient space utilization, avoids congestion, and improves user experience.  

---

Project Objectives 
The main goals of the Parking System project are:  
1. To provide a simple and effective way to manage parking slots dynamically.
2. To enable users to park and retrieve cars without hassle by using their license plate numbers. 
3. TOtrack the available parking slots and ensure that users can only park if there are available slots. 
4. To provide a fast and user-friendly way to view all parked cars in the system. 

---

Features and Functionalities  

1. Dynamic Slot Management
- Users can enter the total number of parking slots at the beginning.  There is an update for available slots in case a car has been parked and removed from the slots. 

2. Park a Car 
  - Users may enter the license plate number of a car to park it.
- The system checks if a parking slot is available before parking.  
   - If parking slots are full, a message informs the user that no spaces are available.  

3. Remove a Car  
   - Users can remove a parked car by entering its license plate number.
- The car is checked if parked before removing.  
   - Slots that are free increase when a car is removed.  


4. View Parked Cars  
   - Users can view all currently parked cars in the system.  
   - If no cars are parked, an appropriate message is presented to the user.

5. Menu-Driven Interface for Users to Choose Their Actions
 The system offers the user a menu-driven interface in order to let the user select an action to be performed.
 The available choices are parking a car, taking away a car, listing out the parked cars, or quitting the system.

---

Implementation Requirements

1. Programming Language: Java
2. Data Structure Used: `ArrayList<String>` to store parked cars
3. Input/Output Handling:
- Scanner is used to take dynamic user inputs.  
   - Print statements are used to guide users and print the appropriate messages.  
4. Loop Structure:  
   - The system runs in an infinite loop (`while(true)`) until the user wants to exit.  
   - A `switch-case` statement is used for the user interaction.

1. Initialization  
   - The system starts by prompting the user to enter the total number of parking slots.  
   - The number of available slots is initialized accordingly.  

2. User Interaction (Main Menu) 
   - The system continuously presents the menu until the user chooses to exit.
- The user can choose options with numbers (for example, `1` to park and `2` to collect).
 
3. Parking a Car (`parkCar()` Method)
   If there is an available parking slot, the application asks the user to input the license plate number of the car.
   The car's license plate is added to the `ArrayList`, and the count of free slots decreases.

4. Deleting a Car (`removeCar()` Method) 
   The system prompts the user to input the license plate number of the car to delete. 
   If the car exists in the list, it is deleted, and available slots increase.

5. Viewing Parked Cars (`viewParkedCars()` Method) 
   The system will display all the parked cars if there are any.
- If no cars are parked, an appropriate message is displayed.  

---

Example Run 

Enter the total number of parking slots:
5

What would you like to do?
1. Park a car
2. Remove a car
3. View parked cars
4. Exit
Choice: 1

Enter the license plate number of the car:
ABC-123
Car parked successfully. Available slots: 4

What would you like to do?
1. Park a car
2. Remove a car
3. View parked cars
4. Exit
Choice: 3

Parked cars:
ABC-123

What do you want to do?
1. Park a car
2. Unpark a car
3. Show parked cars
4. Exit
Select 2

Input the license number of the car to be unparked:
ABC-123
Car unparked successfully. Remaining slots: 5
The Parking System is a simple and efficient solution for parking space management. It tracks the parked cars properly, avoids over-parking, and enhances user experience through a structured and interactive console application. The modular structure of the code makes it easy to expand and integrate with more advanced parking management systems in the future.
The Parking System is a direct and efficient method of managing parked spaces. Proper tracking of cars, prevention from over-parking, and overall improvement in the user experience have been achieved using a structured, interactive console application. The structure of the code is modular; hence, adding more advanced features of parking management systems can easily be done later.

