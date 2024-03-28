# Create and Manage Microsoft Entra ID Users in the Portal

**There are 4 objectives with this lab:**
* Create Microsoft Entra ID User Accounts
* Modify a Microsoft Entra ID User Account
* Revoke Access to a Microsoft Entra ID User Account
* Delete a Microsoft Entra ID User Account


## Create Microsoft Entra ID User Accounts

Once I was logged into the portal, I navigated to the Entra ID section of the portal by typing Microsoft Entra ID in the search bar.

![Image](EntraID1.png)

Once I was in Entra ID, I found the `Users` blade on the left side. 

![Image](EntraID2.png)

Creating a user is pretty straightforward. I clicked on `New User` at the top of the page and put in the name for my users. We also have to give them a password and Azure conveniently will generate a password for you. 

![Image](EntraID3.png)

![Image](EntraID4.png)

We had to create two users so I created Ayanna Will and Edward Von <3. That completes the first objective

![Image](EntraID5.png)

## Modify a Microsoft Entra ID User Account

In PowerShell, we can use simple commands such as `AzResourceGroup`, `AzStorageAccount`, and `AzVM` to see the resources that we've created. Our RG was listed and so was the Storage Account that I created for this lab. The AzVM command had no output because we haven't created a VM yet. 

![Image](AzureCreatingVMs3.png)

## Revoke Access to a Microsoft Entra ID User Account

Now, I googled how to create a VM using PowerShell in the Azure Cloud Shell ([link here](https://learn.microsoft.com/en-us/azure/virtual-machines/windows/quick-create-powershell)). The webpage had the following output:

![Image](AzureCreatingVMs4.png)

I only chose a few aspects from these parameters since i didn't create a Vnet. I had to create a username and a password. Once that was finished, Azure created the VM. 

![Image](AzureCreatingVMs5.png)

## Delete a Microsoft Entra ID User Account

We can use the PowerShell cmdlet `AzVM` to list the newly created VM. We can also go to the portal and check it there.

![Image](AzureCreatingVMs6.png)
![Image](AzureCreatingVMs7.png)




## Personal Notes

The " ` " character helps make the input more visible. I will definitely be using that. 

Also, I see why people use variables for different parameters such as the subscription and RG. Copy and pasting wasn't working for me (I was probably just doing it wrong) but it would be nice to assign a variable to each of these values and then put the commands in. It's easier to manage. 
