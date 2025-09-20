# Catalog Item: Network Request

* [cite_start]**Name**: Network Request [cite: 89]
* [cite_start]**Catalogs**: Service Catalog [cite: 90]
* [cite_start]**Category**: Network [cite: 91]

### Description
[cite_start]This catalog item provides a self-service interface for users to submit network service requests[cite: 5].

### Variables

1.  **Is this a new network connection or relocation?**
    * [cite_start]**Type**: Multiple Choice [cite: 105]
    * [cite_start]**Choices**: New, Relocation, None [cite: 107]

2.  **If this is a relocation, Please provide your relocated address here**
    * [cite_start]**Type**: Single Line Text (String) [cite: 108]

3.  **Types of devices**
    * [cite_start]**Type**: Choice [cite: 109]
    * [cite_start]**Choices**: Laptop, Mobiles, Others [cite: 109]

4.  **If anything else, please specify**
    * [cite_start]**Type**: Single Line Text (String) [cite: 112]
    * *Note: This field is conditionally displayed by a UI Policy.*

5.  **Please provide address here**
    * [cite_start]**Type**: Single Line Text (String) [cite: 110]

6.  **Provide device details here**
    * [cite_start]**Type**: Single Line Text (String) [cite: 111]

### Variable Sets
* **Opened on behalf of**
    * [cite_start]**Type**: Reference to User table [cite: 119]
    * [cite_start]*Note: This set also includes fields for Email, Username, and Phone that are auto-populated from the selected user*[cite: 120, 121, 122].
* **Proof of Document**
    * [cite_start]**Type**: Attachment [cite: 123]
