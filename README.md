 ### EXPERIMENT -07 CONFIGURING NETWORK SERVER FOR CONNECTING GATEWAY AND END NODE 
 
## Aim: To  configure  the Network server and end device for traferring data on the network
## Components required: end node stm 32 development kit , dragino LPS8, network server 

## Theory :
When working with sensitive applications or files, saving progress on your local device is a start, but what if you lose access to your device? Network servers address this problem by hosting the files and programs most pertinent to the network and enabling access for consistent, real-time use. 

As a result, personnel or network clients can instantly access important data or tools while also facilitating collaboration between users. Multiple users can make changes to the same program or document for continued development over the course of a project. Via a secure login, remote users can connect to the home network.
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/59db9b76-ddd5-4d6a-9075-8db233f5e479)


In the above graphic, the circle represents an organization network where a network server facilitates collaboration and file sharing between network clients (devices).

 The role of a network server, then, is to provide users with a set of services and access to resources on the network. These features include:

Permissioned access and log-ins for network users Gateway access to the Internet for an organization Centralized location for network resources  Shared access to devices on the network like a printer or a scanner Hosts multi-user apps like email servers, web applications, or CRM

## Procedure :

 1. login to the network server using login link  https://iot.saveetha.in/
 2. Click on the nework server as shown blow 
![Screenshot 2023-10-28 155314](https://github.com/AsinVardhini/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/119417735/04278800-3f41-4f57-b843-aa4f41aba7a3)

 3. click on the add gateway 
 ![Screenshot 2023-10-28 155342](https://github.com/AsinVardhini/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/119417735/c3e96a96-dc0d-4423-b963-0b2b3f475310)
![image](https://github.com/AsinVardhini/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/119417735/8b1c43dc-6499-42a9-8d92-8600983fa663)
![image](https://github.com/AsinVardhini/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/119417735/ddbe5b05-e11b-4122-99a9-6a2640935d19)
![Screenshot 2023-10-28 161430](https://github.com/AsinVardhini/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/119417735/cb9510aa-4185-4a1c-89dc-7c3297a83033)

4. click on the lora options , lora - frequency plan 
5. click on channel s and create a new channel after which you can add a new end device 
![Screenshot 2023-10-28 161623](https://github.com/AsinVardhini/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/119417735/c6afbeb1-5f81-4d0b-8de0-774eec64472e)

6. add the attributesin the end device as  shown below 
![Screenshot 2023-10-28 161811](https://github.com/AsinVardhini/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/119417735/554f0614-9f3e-440c-81bc-f2d074d9bf3b)

7.using AT commands configure end device in serial port utility
AT Commands to set initially (Mandatory)
 AT+FDR // To do factory data reset
 AT+NJM=1 // To set OTAA mode
 AT+ADR=1 // To enable the ADR
 AT+TDC=600000 // To set the default sampling interval as 10 minutes
(Should not give below 5 minutes)
 AT+CLASS=C // To set class C
 AT+DEUI=XX XX XX XX XX XX XX XX // To set Device EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX // To set APP EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX //
To set APP Key
 ATZ // To take effective action on below settings (As like saving)



## OUTPUT 
![image](https://github.com/AsinVardhini/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/119417735/0637ca0e-7891-4956-badf-0f3518da48b2)


## Results: 

  The Network server and end device for traferring data on the network has been accomplished.

