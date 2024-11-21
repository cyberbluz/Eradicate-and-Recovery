# Now it time to Clean up the Mess!!!
![image](https://github.com/user-attachments/assets/3be54560-4314-45df-bfa7-d3cd0dc72e55)
## Referring back to my Playbook and knowing from my investigation that the NSG may be misconfigured, I was able to access the Linux and Windows NSGs and found the 
![image](https://github.com/user-attachments/assets/4d031cdc-024e-47c0-8a1c-8b457e96ea9e)


## Metrics After Hardening / Security Controls
## For the "AFTER" metrics, Network Security Groups were hardened by blocking ALL traffic with the exception of my admin workstation, and all other resources were protected by their built-in firewalls as well as Private Endpoint
![image](https://github.com/user-attachments/assets/e85907eb-3bd5-4f75-8dbf-bc6ad326868e)

![image](https://github.com/user-attachments/assets/b2aacb16-ffaa-44ee-b371-8903aa8f4b62)

## Conclusion

In this project, a mini honeynet was constructed in Microsoft Azure and log sources were integrated into a Log Analytics workspace. Microsoft Sentinel was employed to trigger alerts and create incidents based on the ingested logs. Additionally, metrics were measured in the insecure environment before security controls were applied, and then again after implementing security measures. It is noteworthy that the number of security events and incidents were drastically reduced after the security controls were applied, demonstrating their effectiveness.


![image](https://github.com/user-attachments/assets/c47cdf46-f66f-42a8-b583-34ca0ac18816)
