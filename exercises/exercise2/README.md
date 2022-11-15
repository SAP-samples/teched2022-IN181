# Create an API Proxy

:warning: Disclaimer When completing exercises, some data values or sceenshots may not match what you see on your screen. It is because the tenant you are working with will be unique to you.

In this exercise, we will create an API proxy to connect to a relevant API provider, to discover OData services from SAP Gateway i.e. GWSAMPLE_BASIC. At the end of this exercise, you will have an API proxy for SAP Gateway System. You can use this API proxy to get usage analytics of an API, add detailed documentation about each method, hide specific methods from consumers and API documentations and activate API proxy.

## Creating API Proxy Steps

<b>Objective</b>: After completing these steps you will have created an API Proxy, by doing this, in this exercise you will touch upon Manage phase of API life cycle management which in turns fast tracks adding functionality like traffic management, transformation, documentation without changing the implementation layer.
<br><img src="/exercises/exercise2/images/exA1_APIM_Lifecycle.png" width=60% height=60%>

1. Navigate to APIs Portal - From the Home screen expand the Menu on the left, and expand <b>Design</b>, then click on API. This will bring up the Create API menu.
<br>![](/exercises/exercise2/images/Picture8.png)

2.	Click the Create button
<br>![](/exercises/exercise2/images/exA2_Create_API.png)

3.	From the drop-down select the <b>SAPDeveloperSystemES5</b> API Provider created in the previous exercise.
<br>![](/exercises/exercise2/images/exA2_Select_API_Provider.png)

4.	Click on <b>Discover</b>.
<br>![](/exercises/exercise2/images/exA2_Click_Create.png)

5.	Select the GWSAMPLE_BASIC services by using the search bar to search for <b>sample</b> to narrow down the list. Next click on the radio button for GWSAMPLE_BASIC. Then Click on <b>OK</b>. 
<br>![](/exercises/exercise2/images/exA2_Select_GWSAMPLE.png)

6.	The remaining fields from the API Proxy creation screen are populated from the OData metadata. Enter in the "Version" field <b>TechEd2022</b>. Then click <b>Create</b>.
<br>![](/exercises/exercise2/images/exA2_Finalize_Create_API.png)

7.	Click <b>Save</b>.
<br>![](/exercises/exercise2/images/exA2_Save_API.png)

8.	Note API Proxy status is <b>Not Deployed</b> and not yet accessible. Click on action button from right side and select <b>Deploy</b> to deploy API Proxy.
<br>![](/exercises/exercise2/images/exA2_Deploy_API.png)

Now you have a working, accessible API Proxy for your ECC API.

## Testing the newly created API Proxy

Now that you have created an API proxy on top of an API discovered from the ECC backend and deployed it to make it accessible, it can be helpful to run a quick test to ensure that basic functionality is in place.

1.	To Test your API proxy, expand the menu and expand <b>Test</b> then select <b>APIs</b>.
<br>![](/exercises/exercise2/images/exA2_Menu_TestAPIs.png)

2.	Select your API - in this case <b>GWSAMPLE_BASIC_TechEd2022</b>. Next select <b>Authentication: None</b> and change to <b>Basic Authentication</b>. Enter your ES5 user name and password. Then make sure the BusinessPartnerSet resource is selected from URI drop down.
<br>![](/exercises/exercise2/images/exA2_Test_API.png)

4.	Click the <b>Send</b> Button - you should receive back the sample API Data.
<br>![](/exercises/exercise2/images/exA2_Test_API_Send.png)



## Summary

Congratulations! You've now successfully created and deployed an API Proxy, and tested that it is successfully able to return data from the backend! 

Continue to - [Exercise 3 - Create an API Product](../example3/README.md)

