# Implementation of Coffee Supplychain using Ethereum Smart Contract

This project showcases the journey of coffee beans on blockchain. 

The coffee supply chain is the sequence of activities and process  to bring raw coffee beans from coffee farms to processed coffee in markets. 

#### Problems in Existing System
---
In existing coffee supply chain, the track of procedure of raw coffee beans to processed coffee is not properly maintained on papers and in digital format. Because of this the buyer of coffee remains doubtful about the quality and brand of coffee. As we are not aware about the process, transporters we are also not sure about the quality assurance. Because of this issues in coffee supply chain, People are selling fake coffee by white labeling the names and tags of branded coffees. 

#### What we are providing?
---

- Initial stage in our project is to create new coffee batch which is performed by admin only. 

- After batch initialization farm-inspection is done and the information is updated by farm-inspectors in to the blockchain. 

- After inspection of farm, harvester grows coffee in their farms the update the information of harvesting to the blockchain. 

- When the raw coffee is ready to export , it gets exported by exporting organizations and they also have to update their information into blockchain. 

- After exporting coffee beans can be imported by the processing units and warehouses for doing further process on coffee beans. Importers also have to provide importing information to update it on blockchain. 

- Processors processes the raw coffee beans and update to blockchain. This is how one batch of coffee beans gets completed.

#### In this application we have Six stages
---

1. Admin
2. Farm-Inspector
3. Harvester
4. Exporter
5. Importer
6. Processor

**Admin :** Admin creates new batch which is initial stage of coffee batch.

**Farm-Inspector :**  Farm-inspector are responsible for inspecting coffee farms and updating the information like coffee family, type of seed and fertilizers used for growing coffee

**Harvester :** Harvesters grows coffee beans in their farms and updates the information of crop variety, temperature used and humidity used for growing beans in blockchain.

**Exporter :** Exporters are the organization who exports coffee beans throughout the world. Exporter  adds quantity, destination address, ship name, ship number , estimated date and time and exporter id.

**Importer :** Importers imports the coffee from coffee suppliers and  updates quantity, ship name, ship number , transporters information, warehouse name, warehouse address and the importer's address.

**Processor :** Processors are the organizations who processes raw coffee beans by roasting them on particular temperature and humidity and makes it ready for packaging and to sale into markets. Processor adds the information like quantity, temperature , roasting duration , internal batch number , packaging date time, processor name and processor address.

#### Included Components
---
-  Solidity (Ethereum)
-  Metamask  (Ethereum wallet)
-  Rinkeby test network ( use rinkeby faucet to get ethers on rinkeby network )
-  Infura
-  Truffle
-  IPFS
- Web3JS
-  lampp

#### Prerequisites
---
- Nodejs v9.10 or above
- Truffle v4.1.8 (core: 4.1.8) (http://truffleframework.com/docs/getting_started/installation)
- Solidity v0.4.23
- Metamask (https://metamask.io) /Ganache Wallet
> [Please Note : infura.io provider is used for the demo ]

#### Deployment Steps:
---
`git clone https://github.com/imperialsoftech/okt-token`
`cd okt-token/`
`npm install`

#### Development Screen's
---
#### Login Page
---
![](http://blockchain.imperialsoftech.com/coffee-supplychain-screens/login-new.png)

- Get MetaMask - You can go for this option if you don't have metamask wallet in your chrome or firefox browser and create your own ethereum wallet
- Log in - You can login to user or admin

#### Admin Dashboard
---
![](http://blockchain.imperialsoftech.com/coffee-supplychain-screens/admin.png)

##### Admin Dashboard Displays
- Total Number of Users
- Total Roles
- Total Batches 
- Batches Overview 
- Your Address
- Storage Contract Address
- Coffee Supply Chain Contract Address 
- List of User Roles
- List of all Users in Coffee Supply Chain
- In admin dashboard you will be able to find out total users registered, total number of roles and total coffee batches created. 
- In batches overview section you will be able to find out the progress of each batch. 
- By clicking on button Create Batch , admin will be able to create new batch of coffee beans. 
- In below section of batches overview you can see your address ( admin wallet address), storage contract address, coffee supply chain contract address and user contract address. 
- Below all these addresses, on left side you can find out all the roles available in coffee supply chain and their slugs, on the right side you will find out all users list and their details. 
- Using Create User button  you can add new user into coffee supply chain.

#### Admin Activities
---
##### Create user
![](http://blockchain.imperialsoftech.com/coffee-supplychain-screens/create-user.png)

- Only admin can add new user in coffee supply chain
- In the Add User form admin have to provide basic information of user like User Wallet Address, Username, User Contact Number, Role of User , User Status means the user is activated or deactivated. 
- User can play his role and update information only if he is have activated status. 
- Admin also can provide profile image of user and after submitting form successfully.
- Admin can find out the newly added user in Users List on Admin dashboard.

##### Create New Batch
![](http://blockchain.imperialsoftech.com/coffee-supplychain-screens/create-batch.png)

- To add new coffee beans batch, you can use create batch button in batches overview section in admin dashboard. 
- Here you have to provide basic information of batch like Farmer Registration Number , Farmer’s Name, Farmer’s Address, Exporter Name and Importer Name.
- By submitting Add Batch form you create new batch which can be updated by other roles later. 
- You can find out the details of particular batch in Actions column by pressing on eye icon ( view-batch page )

##### Batch Overview
![](http://blockchain.imperialsoftech.com/coffee-supplychain-screens/admin1.png)

- Get all coffee batch information in batch overview. We get the in at what stage the batch is processing.You can find out progress of batch using eye icon ( view batch page).
- By clicking on the read arrow at the end of batch id, admin can find out the transaction details of that particular batch. 
- Similarly admin can also scan QR-code to find out the transaction details of batch. 
- Coffee Beans Batch States
- --- Processing  :  when the stage is in process
- --- completed   :  when the stage is completed by respective roles
- --- Not Available : Batch is not reached upto this stage

##### Batch Details
###### Batch all process completed
![](http://blockchain.imperialsoftech.com/coffee-supplychain-screens/Batch-Details-complited.png)

###### Batch work in progress
![](http://blockchain.imperialsoftech.com/coffee-supplychain-screens/coffeeSupplychain-inprogress.png)

- In View Batch Page,/ admin will be able to see the progressive information of coffee batch. 
- Here we can get all details of each stage and also the name and address of user who updated the particular stage. 
---

#### User Dashboard
---
![](http://blockchain.imperialsoftech.com/coffee-supplychain-screens/user.png)

#### User Activities
---
##### Update User Profile
![](http://blockchain.imperialsoftech.com/coffee-supplychain-screens/user-update-user.png)

- To update , user profile you can use Update Profile form where you have to fill the information of user like full name of user, his / her contact number and profile image of user. 
- In this form role of user and user status can only be modified by admin, user can not edit this information.

###### Batch Updation by Farm-inspector
![](http://blockchain.imperialsoftech.com/coffee-supplychain-screens/perform-farm-inspection.png)

- To submit the farm inspection information, user’s having role of Farm inspector will be able to see the update button in batch overview.
- By pressing on update button farm inspector can update information by providing Type of Seed, Coffee Family and Fertilizer Used. 
- After successful submit of farm inspectors information batch progress to next step which is harvesting.

###### Batch Updation by Harvester
![](http://blockchain.imperialsoftech.com/coffee-supplychain-screens/perform-harvesting.png)

- Harvester grows coffee beans and after complete nourishing of coffee beans harvester makes the bean ready to export by updating Coffee Variety, Temperature and humidity to blockchain.

###### Batch Updation by Exporter
![](http://blockchain.imperialsoftech.com/coffee-supplychain-screens/perform-exporting.png)

- Exporters sends the raw coffee beans for further process on beans as per demands and they update their own information to blockchain. 
- Once the coffee beans are ready to export, Users having role of Exporters updates the information of Exporting.
- It includes quantity, destination address, ship name, ship number , estimated datetime and exporter id.  
- By pressing submit button on the form, exporting information gets stored on blockchain.

###### Batch Updation by Importer
![](http://blockchain.imperialsoftech.com/coffee-supplychain-screens/perform-importing.png)

- Warehouses and Organizations who process on raw beans imports the raw coffee beans. While importing coffee beans they have to update their information on blockchain.
- Information of Quantity, Ship Name, Ship Number, Transporter Information, Warehouse Name , Warehouse Address and Importer’s Id Number. 
- After importing coffee beans, it goes for processing stage.

###### Batch Updation by Processor
![](http://blockchain.imperialsoftech.com/coffee-supplychain-screens/perform-processing.png)

- At last the Processors have to update the processing information like roasting temperature of coffee and get issued the quality certificate, coffee gets ready to sale out in markets.
- Processing have to fill the information of quantity, temperature, time for roasting, internal batch number, packaging date, processor name and address of processor. 
- And this is how the Coffee Supply Chain completes for one batch.

---

In this way, we can track the progress of coffee bean after each stage in blockchain. 

The stages which are yet not updated in blockchain are denoted using cross sign and the stages which are completed are denoted by right tick sign. 

You can also find out the name, address and contact information of user who updated the particular stage in coffee supply chain.

