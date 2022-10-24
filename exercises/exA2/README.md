# Create an API Proxy

In this exercise, we will create an API proxy to connect to a relevant API provider, to discover OData services from SAP Gateway i.e. GWSAMPLE_BASIC. At the end of this exercise, you will have an API proxy for SAP Gateway System. You can use this API proxy to get usage analytics of an API, add detailed documentation about each method, hide specific methods from consumers and API documentations and activate API proxy.

## Creating API Proxy Steps

After completing these steps you will have created an API Proxy, by doing this, in this exercise you will touch upon Manage phase of API life cycle management which in turns fast tracks adding functionality like traffic management, transformation, documentation without changing the implementation layer.
<br><img src="/exercises/exA2/images/exA1_APIM_Lifecycle.png" width=60% height=60%>

1. Navigate to APIs Portal - From the Home screen under the Quick Actions tile, click on API. This will bring up the Create API wizard.
<br>![](/exercises/exA2/images/exA1_iSuite_Designer_APIs.png)

2.	Click the Create button

3.	From the drop-down select the SAPDeveloperSystemES5 API Provider created in the previous exercise.

4.	Click on <b>Discover</b>.

5.	Select the GWSAMPLE_BASIC services by using the search bar to search for sample. You can use the Search to narrow down the list. Click on OK. The remaining fields from the API Proxy creation screen are populated from the OData metadata. 

6.	Enter in the "Version" field <b>TechEd2022</b>

6.	Click <b>Create</b>.

7.	Click <b>Save</b>.

8.	API Proxy status is <b>Not Deployed</b>. Click on action button from right side and select <b>Deploy</b> to deploy API Proxy.



## Testing the newly created API Proxy

Now that you have created an API proxy from the ECC backend, it can be helpful to run a quick test to ensure that basic functionality is in place.

1.	To Test your API proxy, expand the menu and expand <b>Test</b> then select <b>APIs</b>. 

2.	Select your API - in this case <b>GWSAMPLE_BASIC_TechEd2022</b>. 

3.	Select <b>Authentication: None</b> and change to <b>Basic Authentication</b>. Enter your ES5 user name and password.

4.	Click the <b>Send</b> Button - you should receive back the sample API Data.



## Summary

You've now ...

Continue to - [Exercise 2 - Exercise 2 Description](../ex2/README.md)

