Find the latest Azure RM API Version for a resource provider type
=================================================================

            

When working with the Azure Resource Manager API, it is useful to know the API versions.


Often if you want to implement a new feature, you need to know the API version to call.


Resource Group Templates are one particular place where you will often use the API Version reference


e.g.


 

 

 


This function assists in easily returning the API version for the given provider Type 


E.g. above you can see the:


- ProviderNamespace: Microsoft.Network


- ResourceTypeName: ResourceTypeName


 


When you run the function it will prompt you to select the ProviderNamespace** *** * & ResourceTypeName** *** * from a visible list.


It will then return the API versions.


**Find-AzureRMAPIVersion**


![Image](https://github.com/azureautomation/find-the-latest-azure-rm-api-version-for-a-resource-provider-type/raw/master/providernamespace.png)* *


Then it will prompt for the ResourceTypeName . . * Notice you can filter the search e.g. Net above or Sec below.


![Image](https://github.com/azureautomation/find-the-latest-azure-rm-api-version-for-a-resource-provider-type/raw/master/resourcetypename.png)** *** *


**This will output the Info that you need.**


**  *** ![Image](https://github.com/azureautomation/find-the-latest-azure-rm-api-version-for-a-resource-provider-type/raw/master/apiversions.png)** *** **


You can then subsuquently update your templates or connections to use the latest API Version.


 

 

 


 

 

        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
