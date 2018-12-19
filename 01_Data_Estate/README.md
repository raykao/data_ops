# The Data Estate
The underlying core services/technology stack is of utmost importance.  Before we define what or how our Automation and Security Posture looks like we should design a general architecture and estasblish what we intend to create.  This then defines what gaps we will have, what will the required security levels be and what abstraction/tools we'll need to employ to achiee an repeatable end to end process.

It should be noted that this only deals with core, internal services (on-prem or public/private cloud) for your organization.  This can be extrapolated and reapplied to external or "Edge" (i.e. IoT) computing as well, but will not be explicitly covered in this guide at the time of writing this document (Dec. 2018).  We will explore or add Edge computing at a later date and update this guide accordingly.

The layers we'll examine are:
1. Ingestion
1. Raw Data Storage
1. Raw Data Processing
1. Refined Data Stroage
1. Refined Data Access
1. Data Feedback Loop ("Reingestion"/"Remodeling")

### Things to consider:
- What type of data are we receiving?
    - Structued and Immediately Machine Readable/Parsable (e.g. JSON, YAML, TSV/CSV, XML, etc.)
    - "Unstructued" human readable (e.g. Word Docs, PDF Files, Images/Pictures etc.)
- Is the data streaming?
    - Is it constantly flowing in on a per second/millisecond basis?
- Is it a bulk/batch upload?
    - Done at specific intervals or scheudled time of day?
    - Massive batches? (large amounts of data at sporadic time intervals)
- Does it conform to a known API/Wire Protocol type? (e.g. Kafka, Redis, Mongo etc.)