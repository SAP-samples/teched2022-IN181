# Creating an API Provider

In this exercise you will learn how to create an API Provider to connect to a Gateway Demo System (ES5). At the end of this exercise, you will have an API Provider for Gateway Demo system with link to Catalog Service Collection. You can use this API Provider to discover and manage OData APIs from SAP Gateway and simplify configuration in case of back-end changes


## Step 1: Pre-requisites
In this pre-requisites section, we will first ensure you have a user logon to the Gateway Demo system (ES) : steps 1 to 7 (skip these steps if you already have a logon). 
1. First, we need to create an account on the Gateway system and register for SAP Integration Suite free trial. Skip this step if already have a demo account. 
<br>Create an account on the SAP Gateway Demo system. Details available here: - https://register.sapdevcenter.com/SUPSignForms 
<br>![](/exercises/ex0/images/Picture1.png)

2. You would receive a temporary password and an email to your registered email to reset the password for first logon.
<br>![](/exercises/ex0/images/image.png)
3. Email received for reset of password <br>![](/exercises/ex0/images/Picture3.png)

4. Logon on the SAP Gateway Web UI and change your initial password - https://sapes5.sapdevcenter.com/sap/bc/gui/sap/its/webgui <br>![](/exercises/ex0/images/Picture4.png)
5. Change your password <br>![](/exercises/ex0/images/Picture5.png)
6. Your password is changed <br>![](/exercises/ex0/images/Picture6.png)
7. You should now see the SAP Easy Access screen. Your account is now active and ready for use <br>![](/exercises/ex0/images/Picture7.png)


## Step 2: Log into your SAP Integration Suite application and access API Management 
As a prerequisite for running through this exercise, ensure you have followed the steps as described in exercise 0 and that you have a configured instance of Integration Suite.
1. Log into the Integration Suite application and from the landing page, click on the 'hamburger' menu icon and navigate to 'Configure -> APIs'. <br>![](/exercises/ex0/images/Picture8.png)
2. SAP Gateway also exposes a Business Partner OData API. To connect to the Business Partner OData API and generate necessary documentation in Open API Specification format, we would have to create an API Provider. An API Provider is a logical representation of a backend system where actual services reside. API Provider enables discovery of OData service from SAP Gateway and generation of Open API specification from the OData metadata. In this section we cover the steps to create an API Provider to discover the Business Partner OData APIs. 'API Providers' will be selected by default from the tab menu to see the previously created providers and to create a new one. To create a new provider from this page, click on Create. <br>![](/exercises/ex0/images/Picture9.png)
3. In the overview area, enter the Name and Description for the API Provider.

| Field        | Value           |
| ------------- |-------------|
| Name      | SAPDeveloperSystemES5 |
| Description      | Public SAP Gateway System exposing OData      | 

<br>![](/exercises/ex0/images/Picture10.png)

4. Under the Connection tab, provide the following information.

| Field        | Value           |
| ------------- |-------------|
| Type      | Internet |
| Host      | sapes5.sapdevcenter.com      |
| Port      | 443 |
| Use SSL      | (checked)      | 

<br>![](/exercises/ex0/images/Picture11.png)

5. By providing the Catalog Service Settings, you can search and explore the OData APIs that is available in the specific SAP Gateway account. In Service Collection URL the relative path to OData Catalog Service Collection URL can be provided which is /sap/opu/odata/IWFND/CATALOGSERVICE/ServiceCollection 

Note: - Currently, OData V4 services are not listed for Service Catalog option.

In case you are connecting to a non-default SAP Client then you can specify the sap-client information by using the SAP query parameters (sap-client={your_gateway_client) e.g /sap/opu/odata/IWFND/CATALOGSERVICE/ServiceCollection?sap-client=001 ( where 001 is the sap-client that you would like to connect to)

On the Catalog Service Settings tab, provide the following information

| Field        | Value           |
| ------------- |-------------|
| Path Prefix      | /sap/opu/odata |
| Service Collection URL      | /IWFND/CATALOGSERVICE/ServiceCollection      |
| Authentication Type      | Basic|
| UserName      | (your_GATEWAY_username)      |
| Password      | (your_GATEWAY_password)       |

 <br>![](/exercises/ex0/images/Picture12.png)
6. Click on Save at the top-right side. <br>![](/exercises/ex0/images/Picture13.png)

## Step 3: Test your Settings
1. To Test your settings click on the Test Connection at the top right side  <br>![](/exercises/ex0/images/Picture14.png)
2. The connection test is successful <br>![](/exercises/ex0/images/Picture15.png)
3. To Test your settings, click the Catalog Service Settings tab on the API Provider. Click on the Catalog URL link to see the catalog. <br>![](/exercises/ex0/images/Picture17.png)
4. When the URL was correct you should see a list of services available on the SAP Gateway system (this screen may look different on different browsers). 
Enter your Gateway user and password when prompted by the browser.<br>![](/exercises/ex0/images/Picture16.png)

Note: - After 3 failed attempts, your Gateway will lock.

Congratulations! You have successfully created an API provider!






