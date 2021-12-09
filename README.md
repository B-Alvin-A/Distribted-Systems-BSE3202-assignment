# Distribted-Systems-BSE3202-assignment
JavaRMI
This system has a server HotelServer, client HotelClient, a remote interface RoomManager and the implementation of the remote interface RoomManagerImpl.

More details to the implementation are specified in the Java RMI Exercise document.

2. SOURCE CODE.

This will show the code of the 4 different files to implement in the Java RMI program of the reservation system.
That is the client side, server side, the remote interface and the implementation of the remote interface.

  2.1 RoomManager
 
      This is the interface of the reservation system. This interface performs booking, review of revenue, review of available rooms and review of available guests.

  2.2 RoomManagerImpl

      This implements the remote interface (RoomManager).

  2.3 HotelServer.

      The server runs the remote interface (RoomManager).

  2.4 HotelClient.

      The final module, is the client that makes request to the server that runs the remote interface.

3. IMPLEMENTATION.


To implement, we compile all the java files using javac *. using the linux shell terminal

When compilation is done, we create a stub and skeleton of the RoomManagerImpl by 	using the rmic tool.
This can be done  using the command $ rmic RoomManagerImpl.

Then start the registry, and it has access to all java classes. A server address is specified 	and in this case out server address is 5000.
This is done by running $ rmiregistry 5000.

Then the server is started in this case the HotelServer, then the client is also started in	this case the HotelClient.

These are done in different terminals shell by running $ java *.
