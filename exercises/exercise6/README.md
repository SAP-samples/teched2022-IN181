# Creating an Integration Flow as a REST, OData API and managing as an API Proxy

As a last step in the workflow, let us create an Integration Flow and manage it as an API Proxy  

## Step 1 - Pre-requisites
Make sure that you have the necessary Role Collections to access the Integrations (formerly CPI) section.

## Step 2 - Log into Cloud Integration from the Integration Studio.
1. From the main Studio, navigate to 'Design' > 'Integrations'. <br>![](/exercises/exercise6/images/Picture1.png)

2. Click on 'Import' to import an Integretion Package that we've already prepared for you. The package to import has been placed in the [bundles](../exercise6/bundles/ProductPackage.zip) folder. <br>![](/exercises/exercise6/images/Picture2.png)

3. Once the import is successful, you should see one 'ProductPackage' <br>![](/exercises/exercise6/images/Picture3.png)

4. Navigate to the 'Artefacts' tab and click on 'ProductODataAPI' entity. <br>![](/exercises/exercise6/images/Picture4.png)

5. It opens up the details page, Click on 'Deploy'.  <br>![](/exercises/exercise6/images/Picture5.png)

6. Likewise, perform the same set of steps on the 'PingCheck' resource and deploy the artefact. <br>![](/exercises/exercise6/images/Picture6.png)

7. Head over to 'Monitor' > 'Integrations' > 'Manage Integraton Content' section and make sure the content finishes deployment and is in the 'Started' state. <br>![](/exercises/exercise6/images/Picture7.png)

8. At this point, you may recall that in the first exercise, we did create a Service Instance of the Process Integration Runtime's 'api' plan. Go to BTP cockpit, and gather the service key details of the instance. <br>![](/exercises/exercise6/images/Picture8.png)

9. Go to the 'Studio' main page and click on 'Configure' > 'APIs'. Here we will create an API Provider. <br>![](/exercises/exercise6/images/Picture9.png)

10. Create an API Provider to type 'Cloud Integration'. <br>![](/exercises/exercise6/images/Picture10.png)

11. In the 'Connection' section, make sure you entire the management host, client credentials gathered in step 8. <br>![](/exercises/exercise6/images/Picture11.png)

12. Next, go to APIs > Create and select the newly created API Provider. <br>![](/exercises/exercise6/images/Picture12.png)

13. Click on Disover and the system will display the 2 APIs created in step 7. Selct the ProductODataAPI. <br>![](/exercises/exercise6/images/Picture13.png)

14. Set the authentication type of Basic and key-in your email address and password (S/P User). <br>![](/exercises/exercise6/images/Picture14.png)

15. At this point, you should notice that the Resources section shows the entities from the OData API and all associated Operations. Deploy and API and in order to test it, can may invoke it from a client tool like Postman. <br>![](/exercises/exercise6/images/Picture15.png)
