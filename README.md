# UiPath-ResearchCopyCheck
Process to solve the challenge from https://acme-test.uipath.com/hubfs/WI2%20-%20Research%20Client%20Check%20Copy.pdf
<br>
Process running: LINK WILL BE GENERATED
<br><br>
<h1>SETUP</h1><br>
Unzip the Folder on your computer<br>
Create an Asset with your login and password inside your Orchestrator with the name "ACME_Credential"<br>
![image](https://user-images.githubusercontent.com/20600105/200637754-14edc3c3-9981-4f99-9065-91d268fac943.png)

Create a Queue with the name "Queue_Research_Client_Check"<br>
![orcqueue](https://user-images.githubusercontent.com/20600105/200640288-5b5c88a9-2156-4f42-a326-0cde75da3764.png)

<br>
Run the Dispatcher to login into the ACME system, extract the Work Items and store it into the Queue<br>
Run the Performer to process all the steps from the challenge.<br>
The PDFs will be stored into Data/Input and after the process will be moved to Data/Output<br>
The PNGs will be stored into Data/Input/Saves and after the process will be moved to Data/Output/Saves
