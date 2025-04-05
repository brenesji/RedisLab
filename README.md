# RedisLab
Create ‘Replica Of’ Redis Open Source server on Redis Enterprise Software.

1.	Verify the connectivity to the remote hosts and reply with confirmation (or explain the connection issue you are facing):

 <img width="468" alt="image" src="https://github.com/user-attachments/assets/68572c74-48cf-4cc4-a8a6-0acc67a1eaa8" />


2.	Install standalone Redis Open Source server version 3.0.7 on Server A.

 
<img width="290" alt="image" src="https://github.com/user-attachments/assets/5e03bca1-bbd9-4bd5-b4f5-6b961b2e20cd" />



3.	Use memtier_benchmark, a tool created by Redis Ltd, to load data into the Redis database.

 <img width="468" alt="image" src="https://github.com/user-attachments/assets/4d30647b-61f0-4e54-9d11-b5844cbdcaad" />



4.	Install the latest version of Redis Enterprise Software on Server B.

 <img width="453" alt="image" src="https://github.com/user-attachments/assets/07b46516-53c9-48c2-b8e4-8251f00cf77e" />

 
<img width="468" alt="image" src="https://github.com/user-attachments/assets/fe3e8f2e-ab78-4326-a1f3-7e74e777d5e4" />

5.	Setup Redis Enterprise Software.


<img width="356" alt="image" src="https://github.com/user-attachments/assets/e40d2e5b-47dd-47ed-bcdd-6137c3222a85" />



6.	Create a Redis Database on Redis Enterprise Software

<img width="468" alt="image" src="https://github.com/user-attachments/assets/2ee05739-0e94-49c2-bce3-33321ab60de7" />



7.	Send an email (Reply All) with a few details on how it is going so far.


<img width="468" alt="image" src="https://github.com/user-attachments/assets/c7fc4cb0-c8b1-40b7-97e0-8f9db32070c3" />

 

8.	Enable Unidirectional Replica Of (Active-Passive) between the two Redis servers:

<img width="468" alt="image" src="https://github.com/user-attachments/assets/47edb255-ef90-4bf0-97d7-ee1404876e53" />

<img width="468" alt="image" src="https://github.com/user-attachments/assets/c3baa278-6491-4f2c-a184-fb2513e9c6bd" />


 
9.	Choose any technology to implement the following, using the most efficient Redis Data Type:

•	Insert 100 random (not predictable) values to the Redis Open Source server.
 
cat names.txt | while read word; do redis-cli LPUSH names "$word"; done

<img width="468" alt="image" src="https://github.com/user-attachments/assets/7521923e-3fea-4498-b317-9ae7f70c4be5" />


•	Read and print the values in reverse insertion order from the Redis Enterprise Software.
 

<img width="468" alt="image" src="https://github.com/user-attachments/assets/d8103a4c-acdb-44a8-b0dc-c7f5e7bc6862" />

•	Explain why it is the most efficient Redis Data Type for this task

-	In my opinion the best data type depends on the use case, for this I picked list because it needed to be not predictable hence this way we can read from bottom to top (I could have used sorted sets but this is more like when we need to do ccomparison between values.)

  
10.	Keep the Redis servers running on both hosts after you exit.
Done.


•	Username username: brenes.jairo@hotmail.com
•	password: Redis6379
•	server: https://18.207.176.232:8443/#/sign-in


