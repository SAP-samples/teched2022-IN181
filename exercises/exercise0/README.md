# Provisioning Integration Suite and activating API Management, Cloud Integration

At the end of this exercise you will have an instance of Integration Suite along with API Management and Cloud Integration activated in your BTP SubAccount


## Step 1: Pre-requisites (service entitlements)
You have access to a BTP Account (/cockpit) that has the license entitlements for Integration Suite and other Service Plans (related to Integration Suite). This could either be a BTP Hanatrial free account / a PYAG free-tier account / a production account (if you are already a paying customer).

1. Go to the Entitlements tab in your BTP SubAccount and lauch the 'Add Service Plan' dialog, ensure that you have the 'Integration Suite' entitlement.  <br>![](/exercises/ex0_0/images/Picture1.png)
2. Go to the 'Process Integration Runtime' entitlement and ensure that you have the 'api' and 'integration-flow' service plans checked.  <br>![](/exercises/ex0_0/images/Picture2.png)
3. (Optional for this exercise) Go to the 'API Management, API Portal' entitlement and ensure that you have the 'apiportal-access' and 'on-premise-connectivity' service plans checked.  <br>![](/exercises/ex0_0/images/Picture3.png)
4. (Optional for this exercise) Go to the 'API Management, developer Portal' entitlement and ensure that you have the 'devportal-access' service plan checked.  <br>![](/exercises/ex0_0/images/Picture4.png)


## Step 2: Subscribe to 'Integration Suite' service and enable authorizations to the needed Role Collections
At the end of this step, we would have setup the Integration Suite service and ready to start creating and consuming APIs
1. Navigate to 'Instances and Subscriptions' section and ensure that you have enabled the subscription for 'Integration Suite' If this is not the case, go to 'Create' and create an instance of the entitlement from Step 1.1.  <br>![](/exercises/ex0_0/images/Picture5.png)
2. Create 'service instances' for the 'integration-flow' and 'api' service plans and keep the service keys handy. The official Help documentation guide: https://help.sap.com/docs/CLOUD_INTEGRATION/368c481cd6954bdfa5d0435479fd4eaf/883f025c30a64373b4e4102238a39fd4.html explains how to create instances of the needed service plans.   <br>![](/exercises/ex0_0/images/Picture6.png)
3. Do not access the Integration Suite application yet.! Click on Role Collections. Look for 'Integration_Provisioner' Role Collection, click on Edit and assign your User to this Role Collection. <br>![](/exercises/ex0_0/images/Picture7.png)
4. If you see the 'APIPortal.Administrator', 'APIPortal.Selfservice.Administrator' and 'PI_Administrator' Role Collection, assign your User to these Collections if you do not see them assigned yet. If you do not see these Role Collections, that means Cloud Integration and API Management capabilities haven't been activated yet. You will need to follow point 5 to do so. <br>![](/exercises/ex0_0/images/Picture8.png) <br><br>![](/exercises/ex0_0/images/Picture9.png)
5. <write>
6. Depending on the traffic at this given point of time, the provisioning steps could take a while to successfully complete. Once the onboarding steps are complete, You will be presented with the the Integration Suite Landing page. <br>![](/exercises/ex0_0/images/Picture10.png)
## Next Steps
In the next exercise, we will configure the ES5 backend needed and expose an API. Continue to - [Exercise 1 - Exercise 1 Configure an API Provider](../exercise0/README.md)
