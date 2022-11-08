# UiPath-ResearchCopyCheck
Process to solve the challenge from https://acme-test.uipath.com/hubfs/WI2%20-%20Research%20Client%20Check%20Copy.pdf

Unzip the Folder on your computer
Create an Asset with your login and password inside your Orchestrator with the name "ACME_Credential"
Create a Queue with the name "Queue_Research_Client_Check"

Run the Dispatcher to login into the ACME system, extract the Work Items and store it into the Queue
Run the Performer to process all the steps from the challenge.
The PDFs will be stored into Data/Input and after the process will be moved to Data/Output
The PNGs will be stored into Data/Input/Saves and after the process will be moved to Data/Output/Saves
