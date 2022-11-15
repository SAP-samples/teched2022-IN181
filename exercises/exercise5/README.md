# Consuming an API in API Business Hub Enterprise

We are now ready to consume the API proxy by first registering in the API Business Hub Enterprise as an Application Developer and to be able to create an Application. 

## Step 1 - Pre-requisites

You have followed the previous exercises and attached API Key verification policy in the API Portal.

## Step 2 - Log into API Business Hub Enterprise (ABHE).
1. Ensure that ABHE installation is complete and that you have the right authorizations to publish and manage content. As a first step attempt logging in to ABHE by clicking on API Business Hub Enterprise button in the top right corner menu item

2. You should be able to log into the ABHE home page. If the page asks you to complete the registation process, follow the steps listed. Log off and re-login, if you have to.

3. Go to the BTP Cockpit and in the 'Users' tab, locate your email address and ensure that you have the AuthGroup.API.Admin, AuthGroup.Content.Admin, AuthGroup.Site.Admin role collections assigned. If they are missing, click on 'Assign Role Collection' button and assign these.

4. Re-login to ABHE and now you should be able to see the Product previously published. Click on the Product.

5. In the Product page, you will be able to see the API Proxy 'GWSAMPLE_BASIC'. Familiarize yourself with the API structure by going through the documentation pages. Once are you back in the details page, click on 'Subscribe' > 'Create new Application'

6. Specify and name and click on 'Save'.

7. Make a note of the 'Application Secret' and 'Application Key'. This will come in handy while invoke the API.

8. Now we are ready to test the API. In order to do so, you may either use the inbuilt 'Test Console' or an external client like Postman / Curl.

9. Head back to the API Portal and copy the URL of the API Proxy created before (GWSAMPLE_BASIC). 

10. Load the API in your preferred test tool (Postman demonstrated here), enter 'APIKey' and the value of the Applicaton key in the 'Headers' section and click 'Send'. 

11. You will see a '401 unathorized' error. This error comes directly from the backend. At this point, we have successfully passed the API Key verification step. 

12. To to the 'Authentication' section and pass the username, password credentials of the backend's and you should be able to see a successful response from the backend


