# Investigations

**THE CISSP TOPICS COVERED IN  THIS CHAPTER INCLUDE:**

- **Domain 1.0: Security and Risk Management**
    - 1.5 Understand requirements for investigation types (e.g., administrative, criminal, civil, regulatory, industry standards)

- **Domain 7.0: Security Operations**
    - 7.1 Understand and comply with investigations
        - 7.1.1 Evidence collection and handling
        - 7.1.2 Reporting and documentation
        - 7.1.3 Investigative techniques
        - 7.1.4 Digital forensics tools, tactics, and procedures
        - 7.1.5 Artifacts (e.g., data, computer, network, mobile device)

As a security professional, you must be familiar with the various types of investigations. These include administrative, criminal, civil, and regulatory investigations, as well as investigations that involve industry standards. You must be familiar with the standards of evidence used in each investigation type and the forensic procedures used to gather evidence in support of investigations.

## Investigations

Every information security professional will, at one time or another, encounter a security incident that requires an investigation. In many cases, this investigation will be a brief, informal determination that the matter is not serious enough to warrant further action or the involvement of law enforcement authorities. However, in some cases, the threat posed or damage done will be severe enough to require a more formal inquiry. When this occurs, investigators must be careful to ensure that proper procedures are followed. Failure to abide by the correct procedures may violate the civil rights of those individual(s) being investigated and could result in a failed prosecution or even legal action against the investigator.

### Investigation Types

Security practitioners may find themselves conducting investigations for a wide variety of reasons. Some of these investigations involve law enforcement and must follow rigorous standards designed to produce evidence that will be admissible in court. Other investigations support internal business processes and require much less rigor.

#### Administrative Investigations

Administrative investigations are internal investigations that examine either operational issues or a violation of the organization's policies. They may be conducted as part of a technical troubleshooting effort or in support of other administrative processes, such as human resources disciplinary procedures.

Operational investigations examine issues related to the organization's computing infrastructure and have the primary goal of resolving operational issues. For example, an IT team noticing performance issues on their web servers may conduct an operational investigation designed to determine the cause of the performance problems.

#Tip Administrative investigations may quickly transition to another type of investigation. For example, an investigation into a performance issue may uncover evidence of a system intrusion that may then become a criminal investigation.

Operational investigations have the loosest standards for collection of information. They are not intended to produce evidence because they are for internal operational purposes only. Therefore, administrators conducting an operational investigation will only conduct analysis necessary to reach their operational conclusions. The collection need not be thorough or well documented, because resolving the issue is the primary goal.

In addition to resolving the operational issue, operational investigations often conduct a _root cause analysis_ that seeks to identify the reason that an operational issue occurred. The root cause analysis often highlights issues that require remediation to prevent similar incidents in the future.

Administrative investigations that are not operational in nature may require a stronger standard of evidence, especially if they may result in sanctions against an individual. There is no set guideline for the appropriate standard of evidence in these investigations. Security professionals should consult with the sponsor of the investigation as well as their legal team to determine appropriate evidence collection, handling, and retention guidelines for administrative investigations.

#### Criminal Investigations

Criminal investigations, typically conducted by law enforcement personnel, investigate the alleged violation of criminal law. Criminal investigations may result in charging suspects with a crime and the prosecution of those charges in criminal court.

Most criminal cases must meet the _beyond a reasonable doubt_ standard of evidence. Following this standard, the prosecution must demonstrate that the defendant committed the crime by presenting facts from which there are no other logical conclusions. For this reason, criminal investigations must follow strict evidence collection and preservation processes.

#### Civil Investigations

Civil investigations typically do not involve law enforcement but rather involve internal employees and outside consultants working on behalf of a legal team. They prepare the evidence necessary to present a case in civil court resolving a dispute between two parties.

Most civil cases do not follow the beyond a reasonable doubt standard of proof. Instead, they use the weaker _preponderance of the evidence_ standard. Meeting this standard simply requires that the evidence demonstrate that the outcome of the case is more likely than not. For this reason, evidence collection standards for civil investigations are not as rigorous as those used in criminal investigations.

#### Regulatory Investigations

Government agencies may conduct regulatory investigations when they believe that an individual or corporation has violated administrative law. Regulators typically conduct these investigations with a standard of proof commensurate with the venue where they expect to try their case. Regulatory investigations vary widely in scope and procedure and are often conducted by government agents.

#### Industry Standards

Some regulatory investigations may not involve government agencies. These are based on industry standards, such as the Payment Card Industry Data Security Standard (PCI DSS). These industry standards are not laws but are contractual obligations entered into by the participating organizations. In some cases, including PCI DSS, the organization may be required to submit to audits, assessments, and investigations conducted by an independent third party. Failure to participate in these investigations or negative investigation results may lead to fines or other sanctions. Therefore, investigations into violations of industry standards should be treated in a similar manner as regulatory investigations.

**Key Points:**
1. **<mark style="background: #FFF3A3A6;">Administrative</mark> Investigations vs. <mark style="background: #BBFABBA6;">Criminal</mark> Investigations:**
    - **Purpose**: Administrative investigations are <mark style="background: #FFF3A3A6;">primarily focused on resolving operational issues or policy violations within an organization</mark>, while criminal investigations <mark style="background: #BBFABBA6;">aim to gather evidence for potential prosecution of a crime</mark>.
    - **Standard of Evidence**: Administrative investigations typically have lower standards of evidence than criminal investigations (e.g., "<mark style="background: #FFF3A3A6;">more likely than not</mark>" vs. "<mark style="background: #BBFABBA6;">beyond a reasonable doubt</mark>").
    - **Scope and Procedure**: Administrative investigations may be <mark style="background: #FFF3A3A6;">less rigorous</mark> in terms of evidence collection and preservation, as they are not focused on producing admissible evidence for criminal proceedings.
    
2. **<mark style="background: #FFF3A3A6;">Administrative</mark> Investigations vs. <mark style="background: #ABF7F7A6;">Civil</mark> Investigations:**
    - **Purpose**: Both administrative and civil investigations are focused on resolving disputes or issues within an organization, but civil investigations are <mark style="background: #ABF7F7A6;">typically more focused on financial compensation or other remedies</mark>.
    
3. **<mark style="background: #FFB8EBA6;">Regulatory</mark> Investigations vs. <mark style="background: #FFB86CA6;">Industry</mark> Standards:**
    - **Purpose**: Regulatory investigations are <mark style="background: #FFB8EBA6;">conducted by government agencies</mark> to ensure compliance with laws or regulations, while industry standards are <mark style="background: #FFB86CA6;">contractual obligations between participating organizations</mark>.
    - **Scope and Procedure**: Regulatory investigations may have different procedures and standards for evidence collection and analysis compared to other types of investigations, as they are <mark style="background: #FFB8EBA6;">focused on ensuring compliance with legal requirements</mark>. Industry standards may also have different procedures and standards, but t<mark style="background: #FFB86CA6;">hey are contractual obligations rather than legal requirements</mark>.

#### Electronic Discovery

In legal proceedings, each side has a duty to preserve evidence related to the case and, through the discovery process, share information with their adversary in the proceedings. This discovery process applies to both paper records and electronic records, and the electronic discovery (or eDiscovery) process facilitates the processing of electronic information for disclosure.

The <mark style="background: #FFF3A3A6;">Electronic Discovery Reference Model (EDRM)</mark> describes a standard process for conducting eDiscovery with nine aspects:

- **Information Governance** - Ensures that information is well organized for future eDiscovery efforts

- **Identification** - Locates the information that may be responsive to a discovery request when the organization believes that litigation is likely

- **Preservation** - Ensures that potentially discoverable information is protected against alteration or deletion

- **Collection** - Gathers the relevant information centrally for use in the eDiscovery process

- **Processing** - Screens the collected information to perform a “rough cut” of irrelevant information, reducing the amount of information requiring detailed screening

- **Review** - Examines the remaining information to determine what information is relevant to the request and removes any information protected by attorney-client privilege

- **Analysis** - Performs deeper inspection of the content and context of remaining information

- **Production** - Places the information into a format that may be shared with others and delivers it to other parties, such as opposing counsel

- **Presentation** - Displays the information to witnesses, the court, and other parties

#Tip For more information on the EDRM, see [http://edrm.net/resources/frameworks-and-standards/edrm-model](http://edrm.net/resources/frameworks-and-standards/edrm-model)`

![[Pasted image 20240715222013.png]]

Conducting eDiscovery is a complex process and requires careful coordination between IT professionals and legal counsel.


  ### Evidence

To successfully prosecute a crime, the prosecuting attorneys must provide sufficient evidence to prove an individual's guilt beyond a reasonable doubt. In the following sections, we'll explain the requirements that evidence must meet before it is allowed in court, the various types of evidence that may be introduced, and the requirements for handling and documenting evidence. The items of evidence that you maintain and may use in court are also known as _artifacts_ and may include physical devices, such as computers, mobile devices, and network devices, the logs and data generated by those devices, and many other forms of evidence.

#Tip The National Institute of Standards and Technology's Guide to Integrating Forensic Techniques into Incident Response (SP 800-86) is a great reference and is available at [https://csrc.nist.gov/pubs/sp/800/86/final](https://csrc.nist.gov/pubs/sp/800/86/final)`.

#### Admissible Evidence

There are **three** basic requirements for evidence to be introduced into a court of law. To be considered _<mark style="background: #FFF3A3A6;">admissible evidence</mark>, it must meet all three of these requirements, as determined by a judge, prior to being discussed in open court:

- The evidence must be _<mark style="background: #BBFABBA6;">relevant</mark>_ to determining a fact.
- The fact that the evidence seeks to determine must be _<mark style="background: #BBFABBA6;">material</mark>_ (that is, related) to the case.
- The evidence must be _<mark style="background: #BBFABBA6;">competent</mark>, meaning it must have been obtained legally. Evidence that results from an illegal search would be inadmissible because it is not competent.

#### Types of Evidence

Many different types of evidence can be used in a court of law. Depending on the reference you consult, these may be grouped in many different ways. However, you should be familiar with these **four** major categories: real evidence, documentary evidence, testimonial evidence, and demonstrative evidence. Each has slightly different additional requirements for admissibility.

**<mark style="background: #FFF3A3A6;">Real Evidence</mark>** _Real evidence_ (also known as _object evidence_) consists of things that may actually be brought into a court of law. In common criminal proceedings, this may include items such as a murder weapon, clothing, or other physical objects. In a computer crime case, real evidence might include seized computer equipment, such as a keyboard with fingerprints on it or a hard drive from a malicious actor's computer system. Depending on the circumstances, real evidence may also be _conclusive evidence_, such as DNA, that is incontrovertible.

**<mark style="background: #FFF3A3A6;">Documentary Evidence</mark>** _Documentary evidence_ includes any written items brought into court to prove a fact at hand. This type of evidence must also be authenticated. For example, if an attorney wants to introduce a computer log as evidence, they must bring a witness (for example, the system administrator) into court to testify that the log was collected as a routine business practice and is indeed the actual log that the system collected.

Two additional evidence rules apply specifically to documentary evidence:

- The _<mark style="background: #BBFABBA6;">best evidence rule</mark>_ states that when a document is used as evidence in a court proceeding, the original document must be introduced. Copies or descriptions of original evidence (known as _secondary evidence_) will not be accepted as evidence unless certain exceptions to the rule apply.
- The _<mark style="background: #BBFABBA6;">parol evidence rule</mark>_ states that when an agreement between parties is put into written form, the written document is assumed to contain all the terms of the agreement and no verbal agreements may modify the written agreement.

If documentary evidence meets the materiality, competency, and relevancy requirements and also complies with the best evidence and parol evidence rules, it can be admitted into court.

##### Chain of Evidence

Real evidence, like any type of evidence, must meet the relevancy, materiality, and competency requirements before being admitted into court. Additionally, real evidence must be authenticated. This can be done by a witness who can actually identify an object as unique (for example, “That knife with my name on the handle is the one that the intruder took off the table in my house and used to stab me”) and unaltered, meaning that it has not been tampered with from the time of collection until the time of use in court.

In many cases, it is not possible for a witness to uniquely identify an object in court. In those cases, a _chain of evidence_ (also known as a _chain of custody_) must be established. The chain of evidence documents everyone who handles evidence—including the police who originally collect it, the evidence technicians who process it, and the lawyers who use it in court. The location of the evidence must be fully documented from the moment it was collected to the moment it appears in court to ensure that it is indeed the same item. This requires thorough labeling of evidence and comprehensive logs, noting who had access to the evidence at specific times and the reasons they required such access.

When evidence is labeled to preserve the chain of custody, the label should include the following types of information about the collection:

- General description of the evidence
- Time and date the evidence was collected
- Exact location the evidence was collected from
- Name of the person collecting the evidence
- Relevant circumstances surrounding the collection

Each person who handles the evidence must sign the chain of custody log, indicating the time they took direct responsibility for the evidence and the time they handed it off to the next person in the chain of custody. The chain must provide an unbroken sequence of events accounting for the evidence from the time it was collected until the time of the trial.

**<mark style="background: #FFF3A3A6;">Testimonial Evidence</mark>** _Testimonial evidence_ is, quite simply, evidence consisting of the testimony of a witness, either verbal testimony in court or written testimony in a recorded deposition. Witnesses must take an oath agreeing to tell the truth, and they must have personal knowledge on which their testimony is based. Furthermore, witnesses must remember the basis for their testimony (they may consult written notes or records to aid their memory). Witnesses can offer _direct evidence_: oral testimony that proves or disproves a claim based on their own direct observation. The testimonial evidence of most witnesses must be strictly limited to direct evidence based on the witness's factual observations. However, this does not apply if a witness has been accepted by the court as an expert in a certain field. In that case, the witness may offer an _expert opinion_ based on the other facts presented and their personal knowledge of the field.

##### Hearsay Rule

When a witness offers testimony in court, they must normally avoid the act of hearsay, meaning that they cannot testify about what someone else told them outside of court because the court has no way to substantiate that evidence and find it admissible.

That said, the hearsay rule is one that has many, many exceptions. These include past testimony given by a witness under oath that is no longer available, a statement made against the interest of the person making the statement, a dying utterance, public records, and many other situations.

An extremely important exception to this rule for forensic analysts is the business records exception to the hearsay rule. This says that business records, such as the logs generated by a computer system, may be admitted as evidence if they were made at the time of the event by someone or something with direct knowledge, that they were kept in the course of regular business activity, and that keeping those records is a regular practice of the organization.

Records admitted under the business records exception must be accompanied by the testimony of an individual qualified to show that these criteria were met. This exception is commonly used to introduce system logs and other records generated by computer systems.

**<mark style="background: #FFF3A3A6;">Demonstrative Evidence</mark>** _Demonstrative evidence_ is evidence used to support testimonial evidence. It consists of items that may or may not be admitted into evidence themselves but are used to help a witness explain a concept or clarify an issue. For example, demonstrative evidence might include a diagram explaining the contents of a network packet or showing the process used to conduct a distributed denial-of-service attack. The admissibility of demonstrative evidence is a matter left to the trial court with the general principle that demonstrative evidence must assist the jury in understanding a case.


#### Artifacts, Evidence Collection, and Forensic Procedures

Collecting digital evidence is a tricky process and should be attempted only by professional forensic technicians. The International Organization on Computer Evidence (IOCE) outlines **five principles** to guide digital evidence technicians as they perform media analysis, network analysis, and software analysis in the pursuit of forensically recovered evidence:

1) Upon seizing digital evidence, actions taken should not change that evidence.
2) When it is necessary for a person to access original digital evidence, that person must be forensically competent.
3) All activity relating to the seizure, access, storage, or transfer of digital evidence must be fully documented, preserved, and available for review.
4) An individual is responsible for all actions taken with respect to digital evidence while the digital evidence is in their possession.
5) Any agency that is responsible for seizing, accessing, storing, or transferring digital evidence is responsible for compliance with these principles.

As you conduct forensic evidence collection, it is important to preserve the original evidence. Remember that the very conduct of your investigation may alter the evidence you are evaluating. Therefore, when analyzing digital evidence, it's best to work with a copy of the actual evidence whenever possible. For example, when conducting an investigation into the contents of a hard drive, make an image of that drive, seal the original drive in an evidence bag, and then use the disk image for your investigation.

**<mark style="background: #ABF7F7A6;">Media Analysis</mark>** Media analysis, a branch of computer forensic analysis, involves the identification and extraction of information from storage media. This may include magnetic media (e.g., hard disks, tapes) or optical media (e.g., CDs, DVDs, Blu-ray discs).

Techniques used for media analysis may include the recovery of deleted files from unallocated sectors of the physical disk, the live analysis of storage media connected to a computer system (especially useful when examining encrypted media), and the static analysis of forensic images of storage media.

When gathering information from storage devices, analysts should never access hard drives or other media from a live system. Instead, they should power off the system (after collecting other evidence), remove the storage device, and then attach the storage device to a dedicated forensic workstation, using a _write blocker_. Write blockers are hardware adapters that physically sever the portion of the cable used to connect the storage device that would write data to the device, reducing the likelihood of accidental tampering with the device.

After connecting the device to a live workstation, the analyst should immediately calculate a cryptographic hash of the device contents and then use forensic tools to create a forensic image of the device: a bitwise copy of the data stored on the device. The analyst should then compute the cryptographic hash of that image to ensure that it is identical to the original media contents.

After creating and verifying a forensic image, the original image file should be preserved as evidence. Analysts should create copies of that image (verifying the integrity of the hash) and then use those images for any analysis. This careful process reduces the likelihood of error and ensures the preservation of the chain of custody.

**<mark style="background: #ABF7F7A6;">In-Memory Analysis</mark>** Investigators often wish to collect information from the memory of live systems. This is a tricky undertaking, since it can be difficult to work with memory without actually altering its contents. When gathering the contents of memory, analysts should use trusted tools to generate a _memory dump_ file and place it on a forensically prepared device, such as a USB drive. This memory dump file contains all the contents collected from memory and may then be used for analysis. As with other types of digital evidence, the analyst collecting the memory dump should compute a cryptographic hash of the dump file to later prove its authenticity. The analyst should preserve the original collected dump and work from copies of that dump file.

**<mark style="background: #ABF7F7A6;">Network Analysis</mark>** Forensic investigators are also often interested in the activity that took place over the network during a security incident. This is often difficult to reconstruct due to the volatility of network data—if it isn't deliberately recorded at the time it occurs, it generally is not preserved.

Network forensic analysis, therefore, often depends on either prior knowledge that an incident is under way or the use of preexisting security controls that log network activity. These include:

- Intrusion detection and prevention system logs
- Network flow data captured by a flow monitoring system
- Packet captures deliberately collected during an incident
- Logs from firewalls and other network security devices

When collecting data directly from a network during a live analysis, forensic technicians should use a Session Position Annunciator (SPAN) port on a switch (which mirrors data sent to one or more other ports for analysis) or a network tap, which is a hardware device that performs the same function as a SPAN port. Both of these approaches generate packet dumps without actually altering the network traffic being exchanged between two systems. In cases where this is not possible, the analyst may run a software protocol analyzer on one of the communicating systems, but this approach is not as reliable as using a dedicated hardware device.

After collecting network packets, they should be treated in the same manner as any other digital evidence. The tools creating the packet capture should write them to forensically prepared media. Analysts should compute cryptographic hashes of the original evidence files and work only with copies of those original files.

The task of the network forensic analyst is to collect and correlate information from these disparate sources and produce as comprehensive a picture of network activity as possible.

**<mark style="background: #ABF7F7A6;">Software Analysis</mark>**  Forensic analysts may also be called on to conduct forensic reviews of applications or the activity that takes place within a running application. In some cases, when malicious insiders are suspected, the forensic analyst may be asked to conduct a review of software code, looking for backdoors, logic bombs, or other security vulnerabilities. For more on these topics, see [[Chapter 21]], “Malicious Code and Application Attacks.”

In other cases, forensic analysts may be asked to review and interpret the log files from application or database servers, seeking other signs of malicious activity, such as SQL injection attacks, privilege escalations, or other application attacks. These are also discussed in Chapter 21.

Software analysis may also include the validation of file hash values against known file types. The National Software Reference Library (NSRL) maintained by the National Institute of Standards and Technology includes the cryptographic hash values for over 130 million known applications, making it easier for forensic analysts to detect authentic and manipulated files. For more information on the NSRL, see [www.nist.gov/itl/ssd/software-quality-group/national-software-reference-library-nsrl](http://www.nist.gov/itl/ssd/software-quality-group/national-software-reference-library-nsrl)`.

**<mark style="background: #ABF7F7A6;">Hardware/Embedded Device Analysis</mark>** Finally, forensic analysts often must review the contents of hardware and embedded devices. This may include a review of:

- Personal computers
- Smartphones
- Tablet computers
- Embedded computers in cars, security systems, and other devices

Analysts conducting these reviews must have specialized knowledge of the systems under review. An organization may have to call in expert consultants who are familiar with the memory, storage systems, and operating systems of such devices. Because of the complex interactions between software, hardware, and storage, the discipline of hardware analysis requires skills in both media analysis and software analysis.

##### Locard's Exchange Principle

Locard's exchange principle is the core principle that underlies the field of forensic science. The principle is the work of Dr. Edmond Locard, one of the pioneers of criminal forensics. Locard started a criminal forensics lab in Lyon, France, where he developed the first police laboratory and created many forensics techniques that are the basis for evidence analysis that is still performed today.

Locard's exchange principle, clearly stated, is that <mark style="background: #FFF3A3A6;">“every contact leaves a trace.”</mark> That means that when two objects touch each other, there will be some evidence left behind. That might be a fingerprint, a carpet fiber, a drop of blood or spit, a scratch, or virtually anything else. It then becomes the work of the forensic scientist to discover those traces and interpret them to learn more about a crime that took place.

Most digital forensics experts believe that Locard's principle applies in the digital world as well. Whenever there is contact between two digital objects, that contact leaves a trace. It's up to cybersecurity experts to discover and interpret those traces.

Let's think about this in the context of an example. Suppose that an attacker conducts a SQL injection attack against a website. That attack is going to leave evidence in all of the systems that are touched as part of the attack. Let's think about what some of those places may be.

- First, the attacker used some sort of device to wage the attack. That might be a laptop or desktop computer, a smartphone, a virtual server instance, or something else. That device is going to contain some evidence of the attack. It might have logs that show who was logged into the device, tools that were used in the attack, or the device itself might have physical fingerprints on it or be in an area covered by a security camera.
- Next, the attacker was connected to some network. Maybe they were at home or in an office, or perhaps they waged the attack from a coffee shop or airport Wi-Fi. The network used by the attacker will likely have logs that might reveal important information about the attack.
- That traffic had to cross through several security devices. Certainly, the web server was protected by a network firewall. It might also be protected by an intrusion prevention system, a web application firewall, or other controls. Each of those devices may have identified portions of the attack and maintained records helpful to the investigation. Those might be log entries from the successful attack, or perhaps the attacker tried some other things that didn't work that created important log entries.
- From there, the traffic moved on to the web server hosting the application that was attacked. That server should have logging configured that captured the actual requests received during the attack, and those requests can be used to reconstruct the commands sent by the attacker through the web server to the database server.
- The database server may also have relevant information. If logging is enabled on that server, you'll see the commands executed against the database and be able to reconstruct the attacker's actions.

Those are a ton of different information sources, and they're all brought to us by thinking through an attack in the context of Locard's exchange principle. If we think about how an attack took place and remember that every contact leaves a trace, we'll have plenty of different information sources we can use to piece together our investigation.

