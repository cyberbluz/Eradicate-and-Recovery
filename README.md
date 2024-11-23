# Now it's time to Clean up the Mess!!!
![image](https://github.com/user-attachments/assets/3be54560-4314-45df-bfa7-d3cd0dc72e55)
## Referring back to my Playbook and knowing from my investigation that the NSG may be misconfigured, I accessed the NSG and found the Inbound Security Rule allowing any and all inbound internet traffic. 
![image](https://github.com/user-attachments/assets/4d031cdc-024e-47c0-8a1c-8b457e96ea9e)
****
![image](https://github.com/user-attachments/assets/49934a67-1fd4-42ce-a28c-d36b041b2514)


## I removed the ill-advised security rule, and replaced it with a Hardened rule limiting inbound access to a trusted ip address. I also reviewed the other security rules to ensure no further issues would arise from the NSG.  
![image](https://github.com/user-attachments/assets/4038e946-27e8-4c83-80d8-2df281d0e11e)
## After ensuring the "Success" Alert was indeed a False Positive and no Breach had occurred, I Hardened the NSG and closed out the incident referring several other incidents back to this incident due to their involvement with the same service account ip.
![image](https://github.com/user-attachments/assets/276f66e9-b122-4cb0-9620-cddfd81cad1b)

## I also worked through several Brute Force Attempt alerts and found many were duplicates involving the same ip, but none successfully breached the network.  I carefully mapped the ip addresses looking for connections that would indicate a botnet DDos attack was employed.  Finding no evidence, I closed out the remaining alerts and continued to harden the NSG. 
![image](https://github.com/user-attachments/assets/e4b94837-f06f-46fa-bdc2-5442f9e85c15)


## Metrics After Hardening the Security Controls
## The Network Security Groups were hardened by blocking ALL inbound traffic except for my admin workstation (52.252.187.196), and all other resources were protected by their built-in firewalls as well as Private Endpoint
![image](https://github.com/user-attachments/assets/e85907eb-3bd5-4f75-8dbf-bc6ad326868e)

![image](https://github.com/user-attachments/assets/b2aacb16-ffaa-44ee-b371-8903aa8f4b62)

## Conclusion

In this project, a mini honeynet was constructed in Microsoft Azure and log sources were integrated into a Log Analytics workspace. Microsoft Sentinel was employed to trigger alerts and create incidents based on the ingested logs. Additionally, metrics were measured in the insecure environment before security controls were applied, and then again after implementing security measures. It is noteworthy that the number of security events and incidents were drastically reduced after the security controls were applied, demonstrating their effectiveness.
