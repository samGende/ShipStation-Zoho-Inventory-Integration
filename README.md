# ShipStation Inventory Itegration User Guide

Setup you Zoho inventory integration in two easy steps. 

## ShipStation Setup

### Webhook Setup
Here you'll setup the webhook that informs Zoho an order has been shipped.
1. Navigate to Settings
2. Integration Partners 
3. Click connect Webhooks
4. Click Manage Settings
5. Add a Webhook. Name your Webhook Zoho Inventory.
Then select "On Orders Shipped" within the dropdown. 
Enter the Zoho extension url:"https://f16hlos1sk.execute-api.us-east-2.amazonaws.com/default/shipstation_handler?{org_id}" in the url field. Here org_id should be the org_id given to on subscription.
6. Click Save

### API Access

Now you need to save ShipStations API access tokens to use later in the Zoho setup.

1. Navigate to Settings
2. Account
3. API Settings
4. Select API Version: V1 API
5. Copy the API Key and Secret

## Zoho Setup

Now you need to upload all the Configuration Information with out Zoho Widget

1. Click the ShipStation Inventory Icon on the right sidebar.
2. Copy ShipStation API Key into ShipStation API Key field.
3. Copy ShipStation API Secret into ShipStation API Secret field.
4. Navigate to Settings.
5. Click Incoming Webhooks within Developer & Data. 
6. Hover over makeinvoice, click the blue down arrow, then click "Copy Zapi Key URL".
7. Return to ShipStation inventory Icon and paste the URL in the UpdateInvoice Zapi URL field.
8. Return to Incoming Webhooks and copy the createinvoice Zapi Key URL.
9. Return to ShipStation inventory Icon and paste the URL in the MakeInvoice Zapi URL field.
10. Enter the provided Orginization ID and click "Upload Data". 

ShipStation and Zoho Inventory are now connected!
