# CSCI 560 Spring 2020
# Chapter 2: Data Handling Ethics

# Dr. Ning Zhang

# 1. Introduction
## Definitions
+ Ethics
  - are principles of behavior based on ideas of right and wrong.
+ Ethic principles
  - fairness
  - respect
  - responsibility
  - integrity
  - quality
  - reliability
  - transparency
  - trust
+ Data handling ethics
  - are concerned with how to produce, store, manage, use, and dispose of data in ways that are aligned with ethical principles.
## Data handling ethics are necessary
  - Ethical data handling helps organizations get value from data in long-term
  - Unethical data handling can result in the loss of reputation and customers, and it is illegal in some cases.
## Core concepts of ethical data handling
  - Impact on people
  - Potential for misuse
  - Economic value of data
    + Ethics of data owenership shoud determine how that data value can be accessed and by whom
## Laws and regulatory requirements vs. Ethics
+ There are both legal and ethical reasons to protect data and ensure it is not misused.
## protect data vs. manage data quality
+ There is an ethical imperative not only to protect data, but also to manage its quality.
  - People making decisions, as well as those impacted by decisons, expect data to be complete and accurate.
  - low quality data
    + data that mispresent, is misused, or is misunderstood.
    
## Context Diagram 
+ Review of the Generic Context Diagram of the DAMA-DMBOK Framework

![figure7](../Resources/figure7.png)

+ Data handling ethics context diagram

![figure12](../Resources/figure12.png)

## Summary
+ Many organizations fail to recognize and respond to the ethical obligations inherent in data management.
+ The data enviroment is evolving rapidly. While laws codify some ethical principles, legislation cannot keep up with the risks assocaited with evoluton of the data enviroment.




# 2. Business Drivers
+ An ethical approach to data use is increasingly being recognized as a competive business advantage.  Ethical data handling can 
  - increase the trustworthiness of an organization and the organization's data and process outcomes,
  - create better relationships between the organization and its stakeholders,
  - reduce the risk that data for which the organization is responsible will be misused by employees, customers, or partners,
  - secure data from criminals(Chapter 7)
  - adapt to the influence of  different modles of data ownership, and the emerging roles of Chief Data Officer, Chief Risk Officer, Chierf Privacy Officer, and Chief Analytics Officer.
  
  

# 3. Essential Concepts

## 3.1 Ethical Principles for Data
### Human dignity(starting point for pinciples of data ethics) and automony - **Belmont Report**
+ **Principle 1**: respect for persons
  - repsect their dignity and autonomy as human individuals
+ **Principle 2**:Beneficence
  - minimize risk of harm
  - maximize benefit
+ **Principle 3**:Justice
  - fair and equitable treatment of people 
+ **Principle 4**: Respect for Law and Public Interest (added by The United States epartment of Home Security's **Menlo Report**)

### Privacy - EDPS(European Data Protection Supervisor)
+ Future-oriented regulation of data processing and respect for the rights to privacy and to data protection
+ Accountable controllers who determine personal information processing
+ Privacy conscious engineering and design of data processing products and services
+ Empowered individuals

### Summary
+ Dignity, automony, and privacy is a platform on which a sustainable digital enviroment is shaped.
+ Data governance is a vital tool for ensuring these principles.

## 3.2 Principles Behind Data Privacy Law
+ General Data Protection Regulation of the EU (GDPR, 2016): 
  - rights to acess, rectification of inaccurate data, portiblity
  - rights to object to processing of personal data that may cause damange or distress, and erasure
  - consent that must be affirmative action that is freely gien, specific, informed, and unambiguous.

![GDPR](https://40uu5c99f3a2ja7s7miveqgqu-wpengine.netdna-ssl.com/wp-content/uploads/2018/01/The-7-GDPR-personal-data-processing-principles-view-with-accountability-of-the-controller-for-the-6-principles-added-source-and-courtesy-ServeIT.gif)

+ Canadian Privacy Statutory Obligations
  - applies PIPEDA(Personal Information Protection and Electronic Documents Act) to organizations that collect, use, and sisseminate peronal information in the course of commercial activities.

![PIPEDA](https://image.slidesharecdn.com/personalinformationprotectionandelectronicdocumentsactpipedaandapplicationsecurityandsensitivedataha-170712191102/95/personal-information-protection-and-electronic-documents-act-pipeda-and-implications-for-application-security-and-sensitive-data-handling-in-software-systems-14-638.jpg?cb=1506354909)

+ United States Privacy Program Criteria by the US Federal Trade Commision(FTC, March 2012)

| Principle            | Description of Principle                                                                                                                                                               |
|----------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Notice/Awareness     | Data collectors must disclose their information practices before collecting personal information from consumers.                                                                       |
| Choice/Consent       | Consumers must be given options with respect to whether and how personal information collected from them may be sued for purposes beyond those for which the information was provided. |
| Access/Participation | Consumers should be able to view and contest the accuracy and completeness of data collected about them.                                                                               |
| Integrity/Security   | Data collectors must take reasonable steps to assure that information collected from consumers is accurate and secure from unauthorized use.                                           |
| Enforcement/Redress  | The use of a reliable mechanism to impose sanctions for noncompliance with these fair information practices.                                                                           |

### Summary
+ There is a global trend towards legislative protection of individuals' information privacy.
+ It is important that organizations have policies and guidenlines that enable staff to follow legal requirements.

## 3.3 Online Data in an Ethical Context
+ Ownership of data
+ The rights to be forgotten
+ Identity
  - Having the right to have one indentiy and a coorect identity, and to opt for a private identity.
+ Freedom of speech online

## 3.4 Risks of Unethical Data Handling Practices
+ Data can be misused by
  - judicious data selection
  - manipulation of scale
  - omission of some data points

### 3.4.1 Timing
+ Omission or inclusion of centain data points in a report or activity based on timing

### 3.4.2 Misleading Visualizations
+ Charts and graphs can be used to present data in a misleading manner.
  - changing scale for example

### 3.4.3 Unclear Definitions or Invalid Comparisions
+ The ethnic thing to do, in presenting information, is to provide context that informs its meaning.

### 3.4.4 Bias
+ Data collection for pre-defined result
+ Biases use of data collected
  - some data may be discarded if it does not confirm a pre-determined approach
+ Hunch and search
+ Biased sampling methodology
+ Context and culture

### 3.4.5 Transforming and Integrating Data
+ Data integration presents ethical challenge because data is changed as it moves from system to system. which may present risks:
  - Limited knowledge of data's origin and lineage
  - Data of poor quality
  - Unreliable metadata
  - No documentatoin of data remediation history

### 3.4.6 Obfuscation/Redaction of Data
+ Obfuscation or redacting data is the practice of making information anonymous, or removing sensitive information.
+ The data may be exposed in a downstream activity(analysis or combinaton with other datasets).
  - Data aggregation(see Chapters 7 and 14)
  - Data marking
  - Data masking

## 3.5 Establishing an Ethical Data Culture
+ Establishing a culture of ethical data handling requires 
  - **codes of conducts**: understanding existing practices, defining expected behaviors, codifying tehse in policies and a code of ethics, providing training and oversight to enforce expected behaviors, and strong leadership.
  - **clear communication and governace control**(so that to highlight the problem or stop the process)
  - **formal Organizatinal Change Management(OCM) process** (see Chapter 17)

### 3.5.1 Review Current State Data Handling Practices
+ purpose  
  - to understand the degree they are directly and explicitly connected to ethical and compliance drivers
+ activity
  - identify how well employees understand the ethical implications of existing practices in building and perserving the trust of customers, partners, and other stakeholders.
+ deliverable
  - document ethical principles that underlie the organization's collection, use, and oversight of data, throughout the data lifecycle, including data sharing activities.


### 3.5.2 Identify Principles, Practices, and Risk Factors
+ Formalizing practices is to reduce the risk.
+ Being aware of principes is to imporve priactices.
+ **Principles** should be aligned with risks and practices, and supported by controls
+ Here is one example:
  - guiding principles: People have a right to privacy with respect to information about their health. Therefore, the personal health data of patients should not be accessed except by people who are authorized to access it as part of caring for patients.
  - risk: If there is wide access to the personal health data of patients, then information about individuals could become public knowledge, thereby jeopardizing their right to privacy.
  - practice: Only nurses and doctors will be allowed to access the personal health data of patients and only for purposes of providng care.
  - control: There will be an annual review of all users of the systems that contain personal health information of patients to ensure that only those people who need to have access do have access.

### 3.5.3 Create an Ethical Data Handling Strategy and Roadmap
+ purpose:
  - formalize a strategy to imporve data handling practices.
+ The strategy must express both ethical principles and expected behavior/practices.
  - Values statement
    + What the organization believes in?
    + What is the framework for ethical handling of data and decision making?
  - Ehical data handling principles
    + How an organization approaches challenges presented by data
  - Complicance framework
    + What factors drive organiztional obligation?
  - Risk assesment
    + What are the likelihoon and the implicaitons of specific problems arising within the organization?
  - Training communication
    + Review of the code of ethics
  - Roadmap
    + a timeline with activities that can be approved by management.
  - Approach to auditing and monitoring
    + monitor specific activities to ensure that they are being executed in compliance with ethical principles.


### 3.5.4 Adopt a Socially Responsible Ethical Risk Model
+ **Social responsibility**: not to do harm with the data
+ A **risk model**: 
  - determines whether to execute the project.
  - influences how to execute the project.
+ Example: **Ethical Risk Model for Sampling Projects**

  - Arrow 1: How they select their populations for study
  - Arrow 2: How data will be captured
  - Arrow 3: What activities analytics will focus on
  - Arrow 4: How the results will be made accessible


![figure 13](https://doc.difi.no/nasjonal-arkitektur/kunnskap_bok-navigating-the-labyrinth/media/ethical-risk-model.png)


## 3.6 Data Ethics and Governance
+ Data Ethics and Governance together must keep up-to-date on legal changes, and reduce the risks of ethical impropriety by ensuring employees are aware of their obligations.
+ Data governance must set standards and policies for and provide oversight of dat ahandling practices.
+ Employees must expect fair handling, prtecton from reporting possible breaches, and non-interference in their personal lives.
+ Data

