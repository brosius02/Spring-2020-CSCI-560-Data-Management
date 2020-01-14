# CSCI 560 Spring 2020
# Chapter 1: Data Management
## 1 Introduction
### Data is a vital enterprise asset.
+ Data and information can 
  - give organizations insight about their customers, products, and services.
  - help organizations innovate and reach strategic goals.
+ Few organiztions take advantage of their data.
+ **Data management** helps organizations derive value from data.
+ Data and information are vital assets both in order to derive future value and day-to-day operations.

### Some Concepts
#### Data Management
+ is the development, execution, and supervision of plans, polices, programs, and practices that deliver, control, protect, and enhance the value of data and information assets throughout their lifecycles.

#### Data Management Professional
+ A **Data Management Professional** is any person who works in any facet of data management to meet strategic organizational goals
+ roles of Data Management Professional
  - highly technical
    + database administrators
    + network administrators
    + programmers
  - strategic business
    + data stewards
    + data strategists
    + chief data officer
+ Data management activities
  - technical
  - non-technical(business)
  - Both must be able to collaborate.

## 2. Essential Cocepts
### 2.1 Data
#### Definition
+ Long-standing definitions of **data** emphasize its role in representing facts about the world.
+ In relation to infromation technology, **data** is also understood as infromation that has been stored in digital form.
#### Characteristics
+ Digitization
+ More and more electronic versions of things have been considered as data.
  - videos
  - pictures
  - sound recording
  - documents
  - etc.
+ Volume and velocity
+ Reliable and extensible data management practices are required.
#### Metadata
+ Data is a means of representation, it stands for things other than itself.
+ We need context for data to be meaningful. If we know the  **conventions** of such a system, then we can interpret the data within it.
  - The conventions are often documented in a specific kind of data: Metadata.
#### Multiplicity
+ Multiple choices to represent data
+ Need for Data Architecture, modeling, governace, stwardship, metadata, data quality management...
### 2.2 Data and Information
+ Data: raw material of information
+ Information: data in context
+ Pyramid of Data, information, knowledge, and wisdom

![Pyramid](https://www.ontotext.com/wp-content/uploads/2018/03/DIKW-Pyramid.png)

+ Challenges here
  - It is based on the assumption that data simply exists, but data has to be created.
  - It takes knowledge to create data in the first place.
  - Data and infromation are not separate things, they are dependend on each other. 
    + Data is a form of information
    + Information is a form of data
    + Two terms will be used interchangeably

### 2.3 Data as Organization Asset
+ An **asset**
  - is an economic resource, that can be owned or controlled, and tat holds or produces value.
  - can be converted to money.
+ Monetization of data is becomming increasingly common.
+ Organizations rely on data assets to make more effective decisions and to operate more efficiently.
  - **data-driven** 
    + efficient management
    + professional discipline
    + a partnership of business and technical expertise
+ Data management is not an option, it is the norm.

### 2.4 Data Management Principles

#### Data management characteristics
+ What data an organization has
+ What might be accomplised with the data
+ How best to use data assets to reach organizational goals.
#### Principles needed to balance strategic and operational needs

![figure1](../Resources/figure1.png)

+ Data is an asset with unique properties
  - e.g. Data is not cosumed when it is used
+ The value of data can be and should be expressed in economic terms.
  - There are techniques for measuring data's qualitative and quantitative value
  - There are not standards
  - Organizations should develop consistant ways to quantify that value in order to make better choices.
  - The should also measure both the costs of low quality data and the benefits of high quality data
+ Managing data means managing the quality of data
  - Ensuring that data is fit for purpose is a primary goal of data management.
  - To manage quality, organizations must ensure they understand stakeholders' requirements for quality and measure data against these requirements.
+ It takes Metadata to manage data.
  - Metadata is the definition and knowledge needed to use data.
  - Metadata originates from data management activities.
+ It takes planning to manage data
  - from an architectural and process perspective
+ Data management is cross-functional; it requires a range of skills and expertise.
  - technical skills
  - non-technical skills
  - ability to collaborate
+ Data management requires an enterprise perspective
  - Data management and data governace are intertwined
+ Data management must account for a range of perspectives. (constantly envolve to keep up with)
  - the way data is created
  - the way data is used
  - the data consumers
+ Data management is lifecycle management
  - Data has a lifecycle
  - Data lifecycle is complex
+ Different types of data have different lifecycle charateristics
+ Managing data includes managing the risks associated with data
  - Data can be lost, stolen, or misused.
  - The ethical implications of data use.
  - Data-related risks must be managed as part of the data lifecycle.
+ Data management requirements must drive Information Technology decisions.
  - Data management and information technology are deeply intertwined.
  - Technologies need to serve, not drive, the strategic data needs.
+ Effective data management requires leadership commitment.

### 2.5 Data Management Challenges
Distinct characteristics +  principles => Challenges
#### 2.5.1 Data differs from other assets
+ Differences:
  - Data is not tangible.
  - Data is durable.(it does not wear out, though the value might change.)
  - Data is easy to copy and transport, but not easy to reproduce if it is lost or destroyed.
  - Data can be used for multiple purposes.
  - Data can be used by multiple people at the same time.
  - The use of data beget more data.
+ Challenges:
  - Not easy to put a monetary vaue on data
  - issues that affect data management
+ Benefits
  - Data, indeed, has value.
  - Data is a meta-asset that describe other assets.
  - Data and information are essential to conducting business between and within organizations.
#### 2.5.2 Data valuation
+ Value = Benefit - Cost
+ For data, neither benefit or cost are standardized.
+ General cost and benefit categories
  - Cost of obtaining and storing data
  - Cost of replacing data if it were lost
  - Impact ot organization if data were missing
  - Cost of risk mitigation and potential cost of risks associated with data
  - Cost of improving data
  - Benefits of higher quality data
  - What competitors would pay for data
  - What the data could be sold for
  - Expected revenue from innovative uses of data
+ Chanlleges
  - primary challenge: the value of data is contextual and often temporal
  - Within an organization, certain types of data are likely to be consistently valueable over time.
  - Establishing ways to associate value with data is critical
  - Putting value on data becomes the basis of putting value on data management activities.
#### 2.5.3 Data quality
+ Ensuring that data is of high quality is central to data management.
+ Poor quality data will have negative impact on the decisions of organizations.
  - Organizations spend between 10-30% revenue handling data quality issues.
  - the esitmated cost of poor data in US in 2016 was $3.1 Trillion.
+ Costs come from
  - Scrap and rework
  - work-arounds and hidden correction processes
  - Organizational inefficiencies or low productivity
  - Organizational conflict
  - Low job satisfaction
  - Opportunity costs, including inability to innovate
  - Compliance cost or fines
  - Reputational costs
+ Benifits of high quality data
  - Improve customer experience
  - Higher productivity
  - Reduced risk
  - Ability to act on opportunities
  - Increase revenue
  - Competitive advantage gained from insights on customers, products, and oppotunities.
#### 2.5.4 Planning for Better Data
+ Deriving value from data starts from planning for better data.
+ Decisions about data involve:
  - The way data connects business processes that might otherwise be seen as separate
  - The relationship between business processes and the technology taht support them
  - The design and architecture of system and the data they produce and store
  - The way data might be used to advance organizational strategy
+ Planning for Better Data depends on
  - a strategic approach to architecture, modeling, and other design functions.
  - strategic collaboration between business and IT leadership.
  - the ability to execute effectively on individual projects
+ Challenge
  - organizational pressures and the prennial pressures of time and money
+ Solution
  - Having clarity about the trade-off between long- and short-term goals
#### 2.5.5 Metadata and Data Management
+ Metadata describes
  - what data an organization has
  - what data represents
  - how it is classified
  - where it came from
  - how it moves within the organization
  - how it envoles through use
  - who can and cannot use it
  - whether it is of high quality
+ Challenge:
  - Metadata is a form of data and needs to be managed
  - Metadata often provides a starting points for improvements in data manamgement overall.
#### 2.5.6 Data management is cross-functional
+ range of skills for data management
  - design skills to plan for systems
  - highly technical skills to adiminister hardware and build software
  - data analysis skills to understand issues and problems
  - analytic skills to interpret data
  - language skills to bring consensus to definitions and models
  - strategic thinking to see opportunities to server customers and meet goals
+ challenge
  - getting people with this range of skills and perspectives to recognize how the piece fit together so that they collaborate well as they work toward common goals.
#### 2.5.7 Establishing an enterprise perspective
+ Managing data requires understanding the scope and range of data within an organization.
+ Data is not unique to an organization
+ Data originates in multiple places within an organization
+ Challenge
  - Differences in representational choices
+ Solution
  - data governance
### 2.6 Data Management Strategy


## 3. Data Management Frameworks
### 3.1 Strategic Alignment Model
### 3.2 The Amsterdam Information Model
### 3.3 The DAMA-DMBOK Framework
### 3.4 DMBOK Pyramid (Aiken)
### 3.5 DAMA Data Management Framework Evolved
## 4. DAMA and the DMBOK
+ DAMA: Data Management Association International
+ DMBOK:  The DAMA Guide to the Data Management Body of Knowledage
