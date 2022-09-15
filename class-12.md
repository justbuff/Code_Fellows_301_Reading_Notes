# RADIUS Authentication

Remote Authentication Dial-In User Service (RADIUS) is a networking protocol that authorizes and authenticates users who access a remote network. The client sends the server a RADIUS authentication request. The client is 100% responsible for everything in the request. The server will then start querying the modules in the authorize section and looking in the request for key attributes, such as MS-CHAP-Challenge (for mschap), or CHAP-Challenge (for chap), or EAP-Message (for eap). At the end of authorize, the server will check if anything set the Auth-Type. If nothing did, it immediately rejects the request.

## AAA (Authentication, Authorization and Accounting)

AAA is a standard-based framework used to control who is permitted to use network resources (through authentication), what they are authorized to do (through authorization), and capture the actions performed while accessing the network (through accounting). 

- Authentication: The process by which it can be identified that the user, which wants to access the network resources, valid or not by asking some credentials such as username and password. Common methods are to put authentication on console port, AUX port, or vty lines. 
    
- Authorization: It provides capabilities to enforce policies on network resources after the user has gained access to the network resources through authentication. After the authentication is successful, authorization can be used to determine what resources is the user allowed to access and the operations that can be performed. 

- Accounting: It provides means of monitoring and capturing the events done by the user while accessing the network resources. It even monitors how long the user has access to the network. The administrator can create an accounting method list to specify what should be accounted for and to whom the accounting records should be sent. 
   
## AAA implementation 

- Local database: If we want to use the local running configuration of the router or switch to implement AAA, we should create users first for authentication and provide privilege levels to users for Authorization. 

- ACS server: An external ACS server is used (can be ACS device or software installed on Vmware) for AAA on which configuration on both router and ACS is required. The configuration includes creating a user, separate customized method list for authentication, Authorization, and Accounting. The client or Network Access Server (NAS) sends authentication requests to the ACS server and the server takes the decision to allow the user to access the network resource or not according to the credentials provided by the user. 
