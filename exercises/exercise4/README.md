# Applying Policies to an API


In the previous exerciese you have created API-Provider and API-Proxy. Now let’s manage the API Proxy by applying policies. By doing this, in this exercise you will touch upon Secure and Manage phase of API life cycle management. <br>
You will protect your API Proxy with the “Verify API Key” Policy. This policy allows you to add a simple protection via a so called 'API Key'. Only calls which send a valid API Key along with the main request will be allowed to call the API Proxy

## Step 1 - Pre-requisites

You have followed the previous exercises and created an API Proxy

## Step 2 - Create an API Policy

You have followed the previous exercises and created an API Proxy.

1. In the upper right corner click on Policies to open the policy information for the API.

2. In the Policy Editor, click on Edit.

3. Select the PreFlow from the ProxyEndpoint on the left hand side.

4. Add Verify API Key policy. On the right hand, find the Security Policies section under the Policies pane. Find the Verify API Key policy and click the + next to the policy name.

5. Enter the Policy Name CheckAPIKey and click on Add.

6. Update API Key tag. In the Code Editor found in the bottom pane, look for the <APIKey ... /> tag. Replace the string variable_containing_api_key with request.header.APIKey. Update and save changes.

7. Click on Save to save the changes to the API and enforce the new policies.
