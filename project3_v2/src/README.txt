Stephen Mosby
Kellen Han-Nin Cheng
Aqeel S Bin Rustum
Nai-Wei Chen
CSS558 Sp14 Project3


To run the code on the nodes:

1.  Copy the following files to n01, n02, n03, n04, n05:
		-Server.jar
		
2.	Copy the following files to n06, n07:
		-Client.jar
		
3.  Run the following commands on n01, n02, n03, n04, n05 with the Server.jar, 
	respectively:
		java -jar Server.jar n02, n03, n04, n05
		java -jar Server.jar n01, n03, n04, n05
		java -jar Server.jar n01, n02, n04, n05
		java -jar Server.jar n01, n02, n03, n05
		java -jar Server.jar n01, n02, n03, n04
		
		The arguments for the Server.jar, are the node addresses of servers you
		want to replicate to.

4.	Run the following commands on n06 and n07 with the Client.jar,
	respectively:
		java -jar Client.jar n01
		java -jar Client.jar n03
		
		The argument for the Client.jar, is the address of the server you want 
		to connect to.

To observe atomicity in our two phase commit procedure, you can kill any one of
the servers with the ctrl-c command.