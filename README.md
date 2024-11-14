




## Conclusion

In this project, a mini honeynet was constructed in Microsoft Azure and log sources were integrated into a Log Analytics workspace. Microsoft Sentinel was employed to trigger alerts and create incidents based on the ingested logs. Additionally, metrics were measured in the insecure environment before security controls were applied, and then again after implementing security measures. It is noteworthy that the number of security events and incidents were drastically reduced after the security controls were applied, demonstrating their effectiveness.

It is worth noting that if the resources within the network were heavily utilized by regular users, it is likely that more security events and alerts may have been generated within the 24-hour period following the implementation of the security controls.
![image](https://github.com/user-attachments/assets/c47cdf46-f66f-42a8-b583-34ca0ac18816)
----
----
----
For the "BEFORE" metrics, all resources were originally deployed, exposed to the internet. The Virtual Machines had both their Network Security Groups and built-in firewalls wide open, and all other resources are deployed with public endpoints visible to the Internet; aka, no use for Private Endpoints.

For the "AFTER" metrics, Network Security Groups were hardened by blocking ALL traffic with the exception of my admin workstation, and all other resources were protected by their built-in firewalls as well as Private Endpoint

## Metrics Before Hardening / Security Controls

![image](https://github.com/user-attachments/assets/9cd4666c-0f88-484c-9167-186613a2a9ae)

## Attack Maps Before Hardening / Security Controls
![image](https://github.com/user-attachments/assets/ff9363cc-d4ae-425a-97f7-4cd9aa861cc1)
![image](https://github.com/user-attachments/assets/734bc45f-ee56-432d-9533-d661afd17e30)
![image](https://github.com/user-attachments/assets/09ff8c60-71da-44de-b119-c7af63b60313)

## Metrics After Hardening / Security Controls

![image](https://github.com/user-attachments/assets/e85907eb-3bd5-4f75-8dbf-bc6ad326868e)

![image](https://github.com/user-attachments/assets/b2aacb16-ffaa-44ee-b371-8903aa8f4b62)


## Conclusion

In this project, a mini honeynet was constructed in Microsoft Azure and log sources were integrated into a Log Analytics workspace. Microsoft Sentinel was employed to trigger alerts and create incidents based on the ingested logs. Additionally, metrics were measured in the insecure environment before security controls were applied, and then again after implementing security measures. It is noteworthy that the number of security events and incidents were drastically reduced after the security controls were applied, demonstrating their effectiveness.

It is worth noting that if the resources within the network were heavily utilized by regular users, it is likely that more security events and alerts may have been generated within the 24-hour period following the implementation of the security controls.
![image](https://github.com/user-attachments/assets/c47cdf46-f66f-42a8-b583-34ca0ac18816)
