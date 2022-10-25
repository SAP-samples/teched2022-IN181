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
1. Navigae to 'Instances and Subscriptions' section and ensure that you have enabled the subscription for 'Integration Suite' If this is not the case, go to 'Create' and create an instance of the entitlement from Step 1.1.  <br>![](/exercises/ex0_0/images/Picture5.png)

## Step 3: Test your Settings

