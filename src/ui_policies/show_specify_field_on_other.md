# Catalog UI Policy: Show 'Specify' Field

### Description
[cite_start]This UI policy makes the "If anything else, please specify" field visible only when a user selects "Others" as the device type[cite: 125].

### Configuration

* [cite_start]**Applies to**: A Catalog Item [cite: 131]
* [cite_start]**Catalog Item**: Network Request [cite: 132]
* [cite_start]**When to Apply Condition**: `Types of devices` **is** `Others` [cite: 134]

### UI Policy Action

* **Variable Name**: The variable corresponding to the "If anything else, please specify" question.
* [cite_start]**Visible**: True [cite: 137]
