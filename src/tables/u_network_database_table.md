# Table: Network Database Table

* [cite_start]**Label**: Network Database Table [cite: 143]
* **Name**: u_network_database_table

### Description
[cite_start]This custom table was created to store all records generated from the "Network Request" catalog item[cite: 75].

### Key Columns (Fields)
The table includes the following fields to track request details:

* [cite_start]**Status** [cite: 58]
* [cite_start]**Address** [cite: 58]
* [cite_start]**Device Type** [cite: 58]
* [cite_start]**Relocation Info** [cite: 58]
* [cite_start]**Request Number** (`u_request_number`) [cite: 202]
* [cite_start]**Assigned to** (`u_assigned_to`, Reference to User) [cite: 202]
* [cite_start]**Requested For** (`u_requested_for`, Reference to User) [cite: 202]
* [cite_start]**Approvals** (`u_approvals`, Reference to Approval) [cite: 202]
* [cite_start]**Device Details** (`u_device_details`) [cite: 202]
* [cite_start]**Work status** (`u_work_status`, Choice) [cite: 202]
