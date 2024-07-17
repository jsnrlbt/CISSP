<mark style="background: #FFF3A3A6;">Security management concepts and principles</mark> are inherent elements in a security policy and solution deployment. <mark style="background: #BBFABBA6;">They define the basic parameters</mark> needed for a secure environment. <mark style="background: #BBFABBA6;">They also define the goals and objectives</mark> that both policy designers and system implementers must achieve to create a secure solution.

The <mark style="background: #FFF3A3A6;">5 Pillars of Information Security</mark> are 
- CIA Triad (confidentiality, integrity, availability) - *primary goals and objectives*,
- authenticity, and 
- nonrepudiation. 

# CIA Triad
## Confidentiality
is the concept of the measures used to ensure the protection of the secrecy of data, objects, or resources. <mark style="background: #BBFABBA6;">The goal of confidentiality protection is to prevent or minimize unauthorized access to data</mark>. Confidentiality protections prevent disclosure while protecting authorized access.

Violations of confidentiality
- unauthorized disclosure of sensitive or confidential information are the result of human error, oversight, or ineptitude. 
- can result from the actions of an end user or a system administrator. 
- can also occur because of an oversight in a security policy or a misconfigured security control.

Countermeasures:
- encryption, 
- network traffic padding, 
- strict access control, 
- rigorous authentication procedures, 
- data classification, and 
- extensive personnel training.

Concepts, conditions, and aspects of confidentiality include the following:
- **<mark style="background: #FFF3A3A6;">Sensitivity</mark>** *refers to the quality of information that could cause harm or damage if disclosed.
- **<mark style="background: #FFF3A3A6;">Discretion</mark>** *is a decision where an operator can influence or control disclosure to minimize harm or damage.*
- <mark style="background: #FFF3A3A6;">Criticality</mark> *the level to which information is mission critical. The higher the level of criticality, the more likely the need to maintain the confidentiality of the information.*
- <mark style="background: #FFF3A3A6;">Concealment</mark> *is the act of hiding or preventing disclosure. Concealment is often viewed as a means of cover, obfuscation, or distraction. A related concept to concealment is <mark style="background: #BBFABBA6;">security through obscurity</mark>, which attempts to gain protection through hiding, silence, or secrecy.*
- <mark style="background: #FFF3A3A6;">Secrecy</mark> *is the act of keeping something a secret or preventing the disclosure of information.
- <mark style="background: #FFF3A3A6;">Seclusion</mark> *involves storing something in an out-of-the-way location, likely with strict access controls.
- <mark style="background: #FFF3A3A6;">Isolation</mark> *is the act of keeping something separated from others.*

## Integrity
is the concept of protecting the reliability and correctness of data. <mark style="background: #BBFABBA6;">Integrity protection prevents unauthorized alterations of data</mark>. Properly implemented integrity protection provides a means for authorized changes while protecting against intended and malicious unauthorized activities (such as viruses and intrusions) and mistakes made by authorized users (such as accidents or oversights).

Integrity can be examined from <mark style="background: #ABF7F7A6;">three perspectives</mark>:
- <mark style="background: #BBFABBA6;">Preventing unauthorized subjects from making modifications</mark>
- <mark style="background: #BBFABBA6;">Preventing authorized subjects from making unauthorized modifications</mark>, such as mistakes
- <mark style="background: #BBFABBA6;">Maintaining the internal and external consistency of objects</mark> so that their data is a correct and true reflection of the real world and any relationship with any other object is valid, consistent, and verifiable

For integrity to be maintained on a system, <mark style="background: #BBFABBA6;">controls must be in place to restrict access to data, objects, and resources</mark>. Maintaining and validating object integrity across storage, transport, and processing <mark style="background: #BBFABBA6;">requires numerous variations of controls and oversight.</mark>

Attacks focused on the violation of integrity.
- viruses, 
- logic bombs, 
- unauthorized access, 
- errors in coding and applications, 
- malicious modification, 
- intentional replacement, and 
- system backdoors.

Human error, oversight, or ineptitude accounts for many instances of unauthorized alteration of sensitive information. They can also occur because of an oversight in a security policy or a misconfigured security control.

Countermeasures:
- strict access control, 
- rigorous authentication procedures, 
- intrusion detection systems, 
- object/data encryption, 
- hash verifications, 
- interface restrictions, 
- input/function checks, and 
- extensive personnel training.

Concepts, conditions, and aspects of integrity include the following:
- <mark style="background: #FFF3A3A6;">Accuracy</mark>: Being correct and precise
- <mark style="background: #FFF3A3A6;">Truthfulness</mark>: Being a true reflection of reality
- <mark style="background: #FFF3A3A6;">Validity</mark>: Being factually or logically sound
- <mark style="background: #FFF3A3A6;">Accountability</mark>: Being responsible or obligated for actions and results
- <mark style="background: #FFF3A3A6;">Responsibility</mark>: Being in charge or having control over something or someone
- <mark style="background: #FFF3A3A6;">Completeness</mark>: Having all necessary components or parts
- <mark style="background: #FFF3A3A6;">Comprehensiveness</mark>: Being complete in scope; the full inclusion of all needed elements

## Availability
means authorized subjects are granted timely and uninterrupted access to objects. Often, <mark style="background: #BBFABBA6;">availability protection controls support sufficient bandwidth and timeliness of processing</mark> as deemed necessary by the organization or situation. Availability includes efficient, uninterrupted access to objects and prevention of denial-of-service (DoS) attacks. Availability also implies that the supporting infrastructure—including network services, communications, and access control mechanisms—is functional and allows authorized users to gain access.

For availability to be maintained on a system, controls must be in place to ensure authorized access and an acceptable level of performance, to quickly handle interruptions, provide for redundancy, maintain reliable backups, and prevent data loss or destruction.

Threats to availability. 
- device failure, 
- software errors, and 
- environmental issues (heat, static electricity, flooding, power loss, and so on)
- DoS attacks, 
- object destruction, and 
- communication interruptions.

Many availability breaches are caused by human error, oversight, or ineptitude. They can also occur because of an oversight in a security policy or a misconfigured security control.

Countermeasures:
- designing intermediary delivery systems properly, 
- using access controls effectively, 
- monitoring performance and network traffic, 
- using firewalls and routers to prevent DoS attacks, 
- implementing redundancy for critical systems, and 
- maintaining and testing backup systems. 
- use of fault tolerance features at the various levels of access/storage/security (that is, disk, server, or site) with the goal of eliminating single points of failure to maintain the availability of critical systems.

<mark style="background: #BBFABBA6;">Availability depends on both integrity and confidentiality</mark>. Without integrity and confidentiality, availability cannot be maintained.

Concepts, conditions, and aspects of availability include the following:
- <mark style="background: #FFF3A3A6;">Usability</mark>: The state of being easy to use or learn or being able to be understood and controlled by a subject
- <mark style="background: #FFF3A3A6;">Accessibility</mark>: The assurance that the widest range of subjects can interact with a resource regardless of their capabilities or limitations
- <mark style="background: #FFF3A3A6;">Timeliness</mark>: Being prompt, on time, within a reasonable time frame, or providing a low-latency response


In addition to the CIA Triad, you need to consider a plethora of other security-related concepts and principles when designing a security policy and deploying a security solution. These include the DAD Triad, the risks of overprotection, authenticity, nonrepudiation, and AAA services.

# DAD Triad
The DAD Triad represents the failures of security protections in the CIA Triad. It may be useful to recognize what to look for when a security mechanism fails.
## Disclosure
occurs when sensitive or confidential material is accessed by unauthorized entities. It is a <mark style="background: #BBFABBA6;">violation of confidentiality</mark>.
## Alteration
occurs when data is either maliciously or accidentally changed. It is a v<mark style="background: #BBFABBA6;">iolation of integrity</mark>.
## Destruction
occurs when a resource is damaged or made inaccessible to authorized users (technically, we usually call the latter denial of service). Destruction is a <mark style="background: #BBFABBA6;">violation of availability</mark>.


It may also be worthwhile to know that <mark style="background: #BBFABBA6;">too much security can be its own problem</mark>. Overprotecting confidentiality can result in a restriction of availability. Overprotecting integrity can result in a restriction of availability. Overproviding availability can result in a loss of confidentiality and integrity.

## Authenticity
is the security concept that data is authentic or genuine and originates from its alleged source. This is <mark style="background: #BBFABBA6;">related to integrity</mark> but more closely related to verifying that it is from a claimed origin. When data has authenticity, the recipient can have a high level of confidence that the data is from whom it claims to be and did not change in transit (or storage).

## Nonrepudiation 
ensures that the subject of an activity or who caused an event cannot deny that the event occurred. <mark style="background: #BBFABBA6;">Nonrepudiation prevents a subject from claiming not to have sent a message, not to have performed an action, or not to have been the cause of an event</mark>. It is made possible through identification, authentication, authorization, auditing, and accounting. <mark style="background: #BBFABBA6;">Nonrepudiation can be established using digital certificates, session identifiers, transaction logs, and numerous other transactional and access control mechanisms</mark>. A system built without proper enforcement of nonrepudiation does not provide verification that a specific entity performed a certain action. Nonrepudiation is an essential part of accounting. A suspect cannot be held accountable if they can repudiate the claim against them.

## AAA services 
are a core security mechanism of all security environments. The three As in this abbreviation refer to <mark style="background: #FFF3A3A6;">authentication</mark>, <mark style="background: #FFF3A3A6;">authorization</mark>, and <mark style="background: #FFF3A3A6;">accounting</mark> (or sometimes auditing). However, what is not as clear is that although there are three letters in the acronym, <mark style="background: #BBFABBA6;">it actually refers to five elements: identification, authentication, authorization, auditing, and accounting</mark>.

## Identification
<mark style="background: #BBFABBA6;">is claiming to be an identity when attempting to access a secured area or system.</mark>

A subject must perform identification to start the process of authentication, authorization, and accounting (AAA). <mark style="background: #BBFABBA6;">Providing an identity can involve typing in a username; swiping a smartcard; waving a proximity device; speaking a phrase; or positioning your face, hand, or finger for a camera or scanning device</mark>. Without an identity, a system has no way to correlate an authentication factor with the subject.

Once a subject has been identified (that is, once the subject's identity has been recognized and verified), the identity is accountable for any further actions by that subject. IT systems track activity by identities, not by the subjects themselves. A computer doesn't know one individual from another, but it does know that your user account is different from all other user accounts. Simply claiming an identity does not imply access, authorization, or authority. The identity must be proven before use is allowed or access is granted. That process is authentication.

## Authentication
<mark style="background: #BBFABBA6;">is proving that you are that claimed identity.</mark>

Authentication requires the subject to provide additional information that corresponds to the identity they are claiming. <mark style="background: #BBFABBA6;">The most common form of authentication is using a password</mark>. Authentication verifies the identity of the subject by comparing one or more factors against the database of valid identities (that is, user accounts). The capability of the subject and system to maintain the secrecy of the authentication factors for identities directly reflects the level of security of that system.

<mark style="background: #BBFABBA6;">Identification and authentication are often used together as a single two-step process</mark>. Providing an identity is the first step, and providing the authentication factors is the second step. Without both, a subject cannot gain access to a system—neither element alone is useful in terms of security. In some systems, it may seem as if you are providing only one element but gaining access, such as when keying in an ID code or a PIN. However, in these cases, either the identification is handled by another means, such as physical location, or authentication is assumed by your ability to access the system physically. Both identification and authentication take place, but you might not be as aware of them as when you manually type in both a username and a password.

## Authorization\
<mark style="background: #BBFABBA6;">defines the permissions (i.e., allow/grant and/or deny) of a resource and object access for a specific identity or subject.</mark>

<mark style="background: #BBFABBA6;">Once a subject is authenticated, access must be authorized</mark>. The process of authorization ensures that the requested activity or access to an object is possible, given the rights and privileges assigned to the authenticated identity. In most cases, the system evaluates the subject, the object, and the assigned permissions related to the intended activity. If the specific action is allowed, the subject is authorized. If the specific action is not allowed, the subject is not authorized.

Keep in mind that just because a subject has been identified and authenticated does not mean they have been authorized to perform any function or access all resources within the controlled environment. Identification and authentication are all-or-nothing aspects of access control. Authorization has a wide range of variations between all or nothing for each object within the environment. A user may be able to read a file but not delete it, print a document but not alter the print queue, or log on to a system but not access any resources.

## Auditing
<mark style="background: #BBFABBA6;">is recording a log of the events and activities related to the system and subjects.</mark>

Auditing is the programmatic means by which a subject's actions are tracked and recorded to hold the subject accountable for their actions while authenticated on a system through the documentation or recording of subject activities. It is also the process of detecting unauthorized or abnormal activities on a system. Auditing is recording the activities of a subject and its objects and the activities of application and system functions. Log files provide an audit trail for re-creating the history of an event, intrusion, or system failure. Auditing is needed to detect malicious actions by subjects, attempted intrusions, and system failures. Auditing is also necessary to reconstruct timelines of compromise events, provide evidence for prosecution, and produce problem reports and analyses. Auditing is usually a native feature of operating systems and most applications and services. Thus, configuring the system to record information about specific types of events is fairly straightforward.

#Note Monitoring is part of what is needed for audits, and audit logs are part of a monitoring system, but the two terms have different meanings. Monitoring is a type of watching or oversight, whereas auditing is recording the information into a record or file. It is possible to monitor without auditing, but you can't audit without some form of monitoring.

## Accounting
<mark style="background: #BBFABBA6;">is reviewing log files to check for compliance and violations in order to hold subjects accountable for their actions, especially violations of organizational security policy.</mark>

An organization's security policy can be properly enforced only if accounting is maintained. In other words, you can maintain security only if subjects are held accountable for their actions. Effective accounting relies on the capability to prove a subject's identity and track their activities. Accountability is established by linking an individual to the activities of an online identity through the security services and mechanisms of auditing, authorization, authentication, and identification. Thus, individual accountability is ultimately dependent on the strength of these processes. Without a strong authentication process, there is doubt that the person associated with a specific user account was the actual entity controlling that user account when the undesired action took place.

To have viable accountability, you must be able to support your security decisions and their implementation in a court of law. If you are unable to legally support your security efforts, then you will be unlikely to be able to hold an individual accountable for actions linked to a user account. With only a password as authentication, there is significant room for doubt. Passwords are the least secure form of authentication, with dozens of different methods available to compromise them. However, with the use of multifactor authentication (MFA), such as a password, smartcard, and fingerprint scan in combination, there is very little possibility that any other individual could have compromised the authentication process in order to impersonate the person responsible for the user account.


Although AAA is typically referenced in relation to authentication systems, it is actually a foundational concept for security. <mark style="background: #BBFABBA6;">Missing any of these five elements can result in an incomplete security mechanism.</mark>

