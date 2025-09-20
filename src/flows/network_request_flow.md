# Flow: Network Request Automation

### Description
[cite_start]This flow automates the entire backend process for a submitted network request[cite: 60].

### Configuration

* [cite_start]**Trigger**: Record Created - Triggered when a `sc_req_item` record is created for the "Network Request" catalog item[cite: 61, 247].

### Actions (in order)

1.  **Get Catalog Variables**
    * [cite_start]Retrieves all variables submitted by the user on the "Network Request" form[cite: 63, 248].

2.  **Create Record**
    * [cite_start]Creates a new record in the `Network Database Table` (`u_network_database_table`)[cite: 64, 248].
    * Maps the retrieved catalog variables to the corresponding fields on the new record.

3.  **Ask for Approval**
    * [cite_start]Generates an approval record and assigns it to the appropriate user or group based on defined rules[cite: 65, 248].
    * The flow waits for the approval status (Approved/Rejected) before proceeding.

4.  **Send Email**
    * [cite_start]Sends an email notification to the requester and/or approver to confirm submission, approval, or rejection[cite: 66, 248].
