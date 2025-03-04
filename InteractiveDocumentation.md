# **Interactive Documentation** 
**Objective:** Select **static** technical content and create an interactive educational component for the documentation

**Technical Content:** 
I selected Docusign documentation on how to send a signature request via [email](https://developers.docusign.com/docs/esign-rest-api/how-to/request-signature-email-remote/), [SMS](https://developers.docusign.com/docs/esign-rest-api/how-to/request-signature-sms-whatsapp/), or [template](https://developers.docusign.com/docs/esign-rest-api/how-to/request-signature-template-remote/). 

**Interactive Documentation:**
I combined DocuSign's three workflows into one flowchart to outline the different ways users can send documents for signature requests.

```mermaid
flowchart TD
    A["Obtain 
    OAuth token"] --> B{"Create the
  envelope definition w/
  _**makeEnvelope**_ method"}
    B -- Email --> C["fa:fa-envelope 
    - Create a new HTML document in code. 
    - Recpients identified by name and email"]
    B -- Email Using a Template --> E["fa:fa-book 
    - Specify the ID of the Docusign template. 
    - Provide names and emails of signing parties"]
    B -- SMS --> D["fa:fa-phone 
    - Edit signers phone numbers. 
    - Set the **deliveryMethod** field to _SMS_"]
    C --> F{"Create and 
    send envelope"}
    D --> F
    E --> F
    F -- Email and SMS --> G["**createEnvelope** API method"]
    F -- Email Using a Template --> H@{ label: "-Add access token to request header. **'Authorization : Bearer {ACCESS_TOKEN}'** <br>- Add Account ID to **createEnvelope** method." }
    G --> I{"Signer receives signing link. After signing, signer receives a copy of finalized documents."}
    H --> I

    H@{ shape: rect}
```
