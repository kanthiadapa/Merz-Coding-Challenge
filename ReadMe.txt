Hi,

This is Kanthi and I had interviewed with Tina for Salesforce Developer role on Friday 1/12 at 12:00 PM EST. Below is my solution approach to the coding challenge:

1. I have developed the code in my dev org in trailhead. 
2. I have created a Shipment__c custom object and a Tracking_Number__c field in it. 
3. I have implemented the LWC with a button on it "Get Shipment Status". The user has to click on the button to get the shipment status. 
4. The LWC component can be added to the Shipment page and when the user clicks on the "Get Shipment Status" button, the component fetches the Tracking_Number__c field on the Shipment object (in the getRecord method on @wire) and calls the "getShippingStatus" method with the tracking number as the argument. 
5. The "getShippingStatus" method is in the ShippingService.cls class which has the @AuraEnabled decorator for the getShippingStatus method. 
6. The HTTP request is built in the getShippingStatus method along with the Endpoint and Method name. 
7. The response is then returned to the component which is then stored in teh shippingStatus variable on the component. 
8. I have added the merzcommunities in the named credentials in my org. 
9. The shippingStatus displays the status of the shipment on the LWC component. 
10. Files used for this exercise are
	i. shippingComponent.html
	ii. shippingComponent.js
	iii. shippingComponent.js-meta.xml
	iv. ShippingService.cls