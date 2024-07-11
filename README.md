Gift Shop Application

- How many apps involved 
  This system consists of two applications which are the Delivery application (delivery.java) and the Customer application (customer.java). 

- Brief explanation each apps  
  
  Customer application (customer.java) 
  The purpose of the customer application is to give clients a graphical user interface via which they can make orders at Stella Gift Shop. 
  Order information are sent to the delivery programme, and it processes and verifies user input as well as computes the final cost. 
  The application configures event listeners and initializes the GUI elements. 
  When the "Check Out" button is hit, ActionListener will be added to manage the checkout procedure. 
  It determines the total items and cost. uses an HTTP POST request to provide order details to a local server. 
  Through a socket connection, TCP Socket transmits the identical order data to the delivery application and Link to a MySQL database in order to obtain order information. 

  Delivery application (delivery.java) 
  The delivery application serves as a server, receiving orders from the customer application and displaying them for delivery processing. 
  The Server Socket receives incoming connections on port 9090. 
  Customer (customer application) communication is managed by the Socket. 
  To handle the corresponding actions of the "CLEAR" and "CLOSE" buttons, an ActionListener is attached to them. 

- Architecture/Layer diagram for each of the apps including the middleware 

![WhatsApp Image 2024-07-11 at 10 06 15 PM](https://github.com/SitiSafiahSFG/GiftShopDeliverySystem/assets/149215963/73bbe146-8099-4783-9738-8961f1daa0f8)
