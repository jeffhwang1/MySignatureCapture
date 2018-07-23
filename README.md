# MySignatureCapture Lightning Flow Component

This is a Lightning Component that wraps the Signature Capture Lightning Component from BrightGen listed on the AppExchange. It's useful for demos where you want to showcase signature capture from a Flow and then attach that signature image to a record.

The AppExchange component is included in a managed package so you can't modify the code. That's why this wrapper component was created to:

  - Allow the component to be included in a Lightning Flow.
  - Pass the recordId of the record to capture the signature image on a record.

## Setup Instructions

1. Install the BrightGen AppExchange package in your demo org. The listing for the component can be found here: https://appexchange.salesforce.com/listingDetail?listingId=a0N30000000q5XOEAY

2. Create a new Lightning Component using the Developer Console (File -> New -> Lightning Component). Call it MySignatureCapture.

3. Copy the code in MySignatureCapture.cmp file. 

4. Click on the COMPONENT tab on the far right and Paste the code.

5. You can modify any of the attributes for the BGSIGCAP:SignatureCapture component except recordId. Click Save.

6. Copy the code in MySignatureCapture.design file. 

7. Click on the DESIGN tab on the far right and Paste the code. 

8. Do not modify anything. Click Save.

9. In your Lightning Flow screen, add the the Lightning Component field.

10. Select MySignatureCapture from components. 

11. For input variable, select the recordId to attached the signature image to. (Note: the recordId can be from an input variable or any recordId variable for a record created during the Flow).

12. Save and activate the Flow, and test to ensure the Flow and MySignatureCapture component is working as expected.

Note: Make sure the users of the component have update rights to the object or you will get an error.

## Acknowledgements

Special thanks to Jeff Blanchard for creating the initial Lightning Component wrapper which was then modified to work with Lightning Flows
