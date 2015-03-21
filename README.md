# Group-Expense-Manager
A Java based tool to calculate individual share in group expenses

This tool can be used when you want to calculate how much you need to give or get from other group members.
For example 5 people go out on a trip.Say person A,B,C,D,E. 
And Expenses are like:

1.  Trip road cost : 2000 bucks (A paid 1000,B paid 500,C paid 500)
2.  A,B had snacks : 50 bucks (A paid 50)
3.  B,C,D had drinks : 150 bucks (B paid 150)
4.  hotel cost       : 2500 bucks ( C paid 2500)
  
Here A,B,C,D,E are added to person list file.
There are 3 different groups:
	G5:A,B,C,D,E;
	G2:A,B;
	G3:B,C,D;

For case 1 there are 3 transaction
A paid 1000 in G5 group : G5,A,1000
B paid 500 in G5 group : G5,B,500
C paid 500 in G5 group : G5,C,500

For case 2 there is 1 transaction
A paid 50 in G2 group : G2,A,50

For case 3 there is 1 transaction
B paid 150 in G3 group : G3,B,150

For case 4 there is 1 transaction
C paid 2500 in G5 group : G5,C,2500

So Transaction file will have information like:
G5,A,1000
G5,B,500
G5,C,500
G2,A,50
G3,B,150
G5,C,2500

Important:
	You need to create 3 different files.
		1. Person details file. List all the person name separated by , (comma).
		2. Group details file.List Groups and its members. Members are separated by comma. Group are separated by ; (semi colon), Ex. G1:A,B;G2:B,C;
		3. Transaction detail file. List of transaction which includes person name, his.her share , group . Ex. G3,B,150
	Provide path of file where you want the result. it will be black text file.
	Hit the calculate.
	It will display who has to pay/get how much. It considers all the group expense and combines them. You will get all information in result file.
	
	
