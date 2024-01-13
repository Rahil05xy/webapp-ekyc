IPFS Based File Storage Access Control and Authentication Model for Secure Data Transfer using Blockchain Technique
Online we often share data with others and all the data will be stored at centralized server and if this server hack then all user data will be exposed and services will get disturbed. While sharing data we don’t have fine grained access mechanism which will allow us to control which can access and which users are not allowed to access and to apply fined grained technique Attribute Based Encryption are introduced which will allow user to mention sharing people’s names as attributes and encryption will be done for all those attributes and only those users can decrypt and access the data. Attribute Based Encryption (ABE) solved access control mechanism but still data was managed at single centralized server whose attacker or admin can view and alter data  and in centralized server there is no means of data privacy and immutability.
To avoid above data privacy and security issue Blockchain technology was introduced which has inbuilt support for Distributed Data Storage(data will be stored at multiple nodes, if one down then user can access services from other working nodes) data encryption, verification and data immutable which means data once stored cannot be changed wither by attacker or admin user. Blockchain store each record as block/transaction and then associate each block with unique hash code and while storing new data then Blockchain will verify hash code of all blocks and if data unchanged then it will result into same hash code and verification get successful. Blockchain consider as immutable because of hash code and its verification technique.
Above advantages of Blockchain has inspired author of this paper to manage sharing data securely using Blockchain. Blockchain storage can reduce overhead because of distributed storage access.
In propose paper to manage sharing data securely author employ 5 different techniques which describe below
1)	IPFS: interplanetary file system is used to store encrypted files and this IPFS will saved file in internal memory and returned stored file address as hash code and by using this hash code we can retrieve stored file
2)	Data Owner: This is the user who upload and shared file with other users
3)	Data Requester: This is the user who request files from the data owner and data owner will generate Chebyshev polynomial encryption keys by using or XORING sharing user details and only those users are allowed to access and decrypt file
4)	Smart Contract: this is a small piece of code written in SOLODITY programming which contains functions related to applications like in this smart contract we define function to save and get register user details, access control details, file hash code details etc.
5)	Blockchain: Blockchain is distributed server which manage user data based on functions defined in Smart Contract.
Above mention 5 modules will get executed in 8 different phases which listed below
1)	Setup Phase: Encryption keys parameters will be setup in this phase
2)	Registration Phase: data owner bind encryption keys with data requested using smart contract access control mechanism
3)	Initialization Phase: all data requester list will be initialize for the data owner
4)	Data Encryption & Storage: using above generated keys data will get encrypted using polynomial XOR operations and then store encrypted file in IPFS system and then IPFS will returned hash code address of stored file and then this hash code will get stored in Blockchain. Whenever we need to get file back then we will get Hash code from Blockchain and then that hash code will be input to IPFS to get file data back in Decrypted format
5)	Authentication: this module will assign accessing permission to sharing user to access file
6)	Testing Phase: Generated  authentication will get hashed as permission for user to access file
7)	Access Control Phase: above generated permission will be stored in Blockchain SMART contract as access control
To execute above process we need to use the designed smart contract which can manage above mention access details 
 



