## Nixon Abuku

**Healthcare integration engineer and backend developer.**

I build the plumbing that moves clinical data between hospital systems — HL7 v2 interfaces, Mirth Connect channels, FHIR services — along with the Node.js APIs and PostgreSQL schemas underneath them. Most of my work sits at the point where a message leaves one vendor's system and has to arrive somewhere else intact, in order, and auditable.

Right now I'm focused on FHIR R4 resource modelling, X12 EDI billing workflows, and containerised integration environments.

---

### Toolkit

| Area | Tools |
|---|---|
| **Integration** | HL7 v2 · FHIR R4 · Mirth Connect · MLLP · DICOM MWL · X12 EDI |
| **Backend** | Node.js · Express · Python · REST APIs · RabbitMQ |
| **Data** | PostgreSQL · SQL Server / T-SQL · Power BI |
| **Platform** | Docker · Docker Compose · Git · AWS (boto3) |

---

### Selected work

**[medcore-ehr](https://github.com/nixon-abuku/medcore-ehr)** — A full hospital EHR simulation used as an integration training environment. Eight clinical modules across 19 Docker containers, with ADT, SIU, ORM, ORU, MDM and DFT message flows travelling over MLLP through Mirth Connect, HAPI FHIR R4 for standards compliance, and Keycloak for auth.

**[Healthcare-Integration-Pipeline](https://github.com/nixon-abuku/Healthcare-Integration-Pipeline)** — An end-to-end HL7 v2.3.1 referral pipeline: TCP/IP ingest, Mirth validation and transformation, SQL Server audit and referral tables, and a Power BI dashboard on top. Handles repeating diagnosis segments without data loss; load-tested past 150 messages.

**[Hospital-ADT-Engine](https://github.com/nixon-abuku/Hospital-ADT-Engine)** — A fault-tolerant ADT ingestion engine. Single-threaded FIFO ordering, automatic batch splitting, and non-destructive state transitions so a discharge never overwrites a patient's admission history.

**[hl7-adt-to-dicom-mwl](https://github.com/nixon-abuku/hl7-adt-to-dicom-mwl)** — Converts ADT^A04 radiology registrations into DICOM Modality Worklist entries so imaging staff see the right patient on the right modality.

**[hl7-refi12-to-json-transform](https://github.com/nixon-abuku/hl7-refi12-to-json-transform)** — REF^I12 referral parsing to clean, consumable JSON, built as a Mirth channel with sample messages included.

**[job-tracker-api](https://github.com/nixon-abuku/job-tracker-api)** — REST API on Node.js and PostgreSQL with JWT auth, bcrypt hashing, parameterised queries and server-side ownership checks, so no user can read another's records.

---

Open to healthcare IT and backend engineering work — reach me through GitHub.
