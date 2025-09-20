# Automated Network Request Management in ServiceNow

## 📖 Overview

[cite_start]This project, built on the ServiceNow platform, automates and streamlines the handling of network-related service requests[cite: 4]. [cite_start]The goal is to eliminate manual tracking, improve accuracy, and provide real-time status updates to users and IT staff[cite: 7]. [cite_start]It solves the problem of delays and inconsistencies that arise from manual request handling by providing a standardized, visible, and automated process[cite: 10, 43].

---

## ⚙️ Key ServiceNow Components

### 1. Custom Table: `Network Database Table`
[cite_start]A custom table was created to store and track all network requests[cite: 33, 75].
* [cite_start]**Key Fields**: Status, Address, Device Type, Relocation Info, Request Number, and others[cite: 58, 76].

### 2. Service Catalog Item: `Network Request`
[cite_start]A self-service catalog item allows users to submit requests from the service portal[cite: 5, 27].
* [cite_start]**Name**: Network Request [cite: 89]
* [cite_start]**Category**: Network Services [cite: 28, 91]
* [cite_start]**Variables**: Includes fields for choosing between a "new connection or relocation," specifying device types, addresses, and other details[cite: 48, 49, 50, 51].
* [cite_start]**Variable Set**: An "Opened on behalf of" set is used to auto-populate user details like Email, Username, and Phone[cite: 30, 53, 54].

### 3. Catalog UI Policy
[cite_start]A UI policy dynamically changes the form based on user input[cite: 29].
* [cite_start]**Condition**: When the "Type of device" field is set to "Others"[cite: 125, 134].
* [cite_start]**Action**: The "If anything else, please specify" field is made visible[cite: 51, 137].

### 4. Flow Designer Workflow
[cite_start]An automated flow manages the entire lifecycle of the request[cite: 6, 60].
* [cite_start]**Trigger**: Activates when the "Network Request" catalog item is submitted[cite: 61, 247].
* **Actions**: The flow performs the following sequence of actions:
    1.  [cite_start]Get Catalog Variables from the submission[cite: 63, 248].
    2.  [cite_start]Create a new record in the `Network Database Table`[cite: 64, 248].
    3.  [cite_start]Ask for Approval based on predefined rules[cite: 65, 248].
    4.  [cite_start]Send Email notifications to the requester and approvers[cite: 66, 248].

---

## 🚀 User Journey

[cite_start]The automated process follows a clear user journey[cite: 25, 35]:
1.  User logs into the Service Portal and submits the "Network Request" form.
2.  An approval request is initiated automatically.
3.  The designated approver approves the request.
4.  The request is routed to a technician for fulfillment.
5.  The user is notified once the task is complete.

---

## 🧪 Testing

[cite_start]The solution was validated through functional testing, confirming that[cite: 249]:
* [cite_start]The catalog form and its dynamic fields work as expected[cite: 251, 252].
* [cite_start]The approval workflow is triggered correctly[cite: 253].
* [cite_start]Email notifications are sent successfully[cite: 254].
* [cite_start]Data is accurately created in the custom table[cite: 255].
