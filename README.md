# Problem-on-HashMap-where-data-read-from-.txt-file-and-store-in-Map-and-write-data-into-.txt-file
Write a menu driven program

This application will be used by store owner(admin) or customers. Consider two users are already there in the system for simplicity. 
Admin User (loginId=admin, password = admin)
Customer (loginId=c1, password=c1)

Login is required to perform any operation. Without login, access to any functionality will throw exception. 

Store owner can perform any operation after login.

A customer can browse, order and check status of his order after login. 

Customer can’t access Admin only functionalities like Add Pet, Update Pet, Update order status etc. Accessing Admin only functionality by customer will throw Unauthorized exception

Pet Store Application Menu: 
                            1)Login
                            2)Add new Pet (Admin only functionality)
                            3)Update Pet details (Admin only functionality)
                            4)Display all available pets
                            5)Order a Pet
                            6)Check order status by Order Id
                            7)Update order status (Admin only functionality)
                            8)Exit

Core classes
Pet ( petId, name, category, unitPrice, stocks)
Category is an enum with values like (CAT, DOG, RABBIT, FISH)
Example:
  petId = 101, name=” Bull Dog”, category= DOG, unitPrice= 1000, stocks=50

Order (orderId, petId, quantity, status)
Status is an enum with values like (PLACED, IN_PROCESS, COMPLETED)
Example: 
   orderId=1, petId=101, quantity=5, status=PLACED

Hints :
Create classes, Enums – Pet, Order, Category, Status 
Create required exception classes – AuthenticationException, AuthorizationException, OutOfStockException 
Handle exceptions
Menu creation, using suitable collection classes for storing Pet and Order
Login 
Auto Order Id generation 
Adjusting stocks after an order, order quantity should not be less than available stock 

HighLights of this Project=>                   1)Marker Interface (PetOrderMarkerInterface) which implements in Pet , Order (Classes)
                                               2)Two Classes - a)Pet b)Order
                                               3)Two Enums - a)Category b)OrderStatus
                                               4)Three Custome Exceptions Classes - a)AuthirizationException b)AuthenticationException c)OutOfStockException
                                               5)Fucntional Programing, Stream, Lambda Expression, Method Refrences
                                               6)Exception Handling
                                               7)In End - a) Pet Details write into "PetDetails.txt"  b) Order Details implicitly write into "OrderDetails.txt"
                                                 In Start - a)Pet data read from "PetDetails.txt" and Pet references store into HashMap collection b)Order data read from "OrderDetails.txt" and Order references store into HashMap collection
