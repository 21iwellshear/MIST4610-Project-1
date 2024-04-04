# MIST4610-Project-1
# Team name:
21479 Group 6
# Team Members:
Ireland Wellshear @21iwellshear
Jack Liskey @jackliskey
Ryan Mai @angelmarsh
Ashkon Mokhlesi  @AshkonMokhlesi
Karandeep Singh @ripleykurtz
# Problem Description
The taks at hand is to model and build a relational database for the general workings of a tennis club. MORE.
# Data Model
Explanation of data model: 
![image](https://github.com/21iwellshear/MIST4610-Project-1/assets/150079987/a1778499-57f5-4f6d-a6bb-fcc5bb5faf5c)

# Date Dictionary:

Table: Pro Shop Items
Column Name	Description	Data type	Size	Format	Key?
itemID	PK, unique sequential identifier for each item	INT	2		PK
itemName	Name of the specific item that is sold	VARCHAR	45		
itemDescription	Description of each item	VARCHAR	45		
itemPrice	Price for a guest to purchase an item	INT	3	99	

Table: Transactions
Column Name	Description	Data type	Size	Format	Key?
transactionID	PK, unique sequential identifier for each transaction	INT	4		PK
date	Date when the transaction was made	DATETIME		YYYY/MM/DD	
paymentMethod	Type of payment method (direct transfer, credit card, debit card, check)	VARCHAR	45		
Members_memberID	FK, unique sequential identifier for each member	INT	3		FK - Members
ProShopItems_itemID	FK, unique sequential identifier for each item at the Racket Shop	INT	2		FK - ProShopItems

Table: Members
Column Name	Description	Data type	Size	Format	Key?
memberID	PK, unique sequential identifier for each member	INT	3		PK
monthlyPayment	Amount paid each month by the member	INT	3		
memberName	Name of member 	VARCHAR	45		
startDate	Date of the member's start date at the club	DATETIME		YYYY/MM/DD	
membershipStatus	Statement on whether the member's membership is active, frozen, cancelled 	VARCHAR	45		
phoneNumber	Phone number of the member	VARCHAR	45	9999999999	
Club_clubID	FK, unique sequential identifier for each club	INT	2		FK - Club
dominatHand	The member's dominant hand	VARCHAR	45	Right or Left	
Sponsor_sponsorID	FK, unique sequential identifier for each sponsor	INT	2		FK - Sponsor
address	Street address where the member is located	VARCHAR	45		
city	City where the member is located	VARCHAR	45		
state	State where the member is located	VARCHAR	45		
zipCode	Zip code where the member is located	INT	5		

Table: Sponsor
Column Name	Description	Data type	Size	Format	Key?
sponsorID	PK, unique sequential identifier for each sponsor	INT	2		PK
sponsorName	Name of sponsor	VARCHAR	45		
industry	Name of industry that the sponsor operates in 	VARCHAR	45		
country	Name of the country that the sponsor operates in	VARCHAR	45		

Table: Club
Column Name	Description	Data type	Size	Format	Key?
clubID	PK, unique sequential identifier for each club	INT	2		PK
clubName	Name of club	VARCHAR	45		
address	Street address of the club	VARCHAR	45		
phoneNumber	Phone number of the club	VARCHAR	45	9999999999	
email	Email of the club	VARCHAR	45		
city	City where the club is located	VARCHAR	45		
state	State where the club is located	VARCHAR	45		
zipCode	Zip code where the club is located	INT	5		
![image](https://github.com/21iwellshear/MIST4610-Project-1/assets/150079987/4e11d7b7-36c3-40e0-a911-0e75684c3fb0)

# Queries
1. Description: Determine the total number of coaching sessions conducted by each coach as a percentage of all sessions.
   PICTURE
   - Justification: Understanding the distribution of coaching sessions helps in workload balancing and identifying coaching resource needs.
   - Complexity: JOIN Operation, Aggregation Functions (COUNT), Subquery, GROUP BY Clause, Arithmetic Operations (Percentage Calculation) 
2. Description: List of upcoming tournaments located in China.
     PICTURE
     - Justification: Enables planning for hosting and promoting specific events for China.
     - Complexity: Simple WHERE
3. Description: Find all tennis courts with lighting.
      PICTURE
     - Justification: To schedule evening or night games and training sessions.
     - Complexity: Simple WHERE
4. Description: List winners of tournaments, the prices they won, and the sponsor of the tournament.
      PICTURE
     - Justification: Highlights successful players and their rewards, useful for promotional materials and sponsor relations.
     - Complexity: Complex (Multiple Table Join, GROUP BY)
5. DescriptionL Find all coaches who specialize in training kids age groups and their pay rates.
      PICTURE
     - Justification: Helps allocate coaches based on demand for junior training sessions, optimizing staffing.
     - Complexity: Simple WHERE
6. Description: Find the most purchased items in the pro shop by quantity ordered.
      PICTURE
   - Justification: Identifies best-selling items to manage stock levels effectively.
   - Complexity: Complex (Join, GROUP BY, ORDER BY)
7. Description: Identify Largest Spenders in the Pro Shop and Their Associated Clubs
      PICTURE
   - Justification: For club managers and marketing teams, understanding who the largest spenders are and their club affiliations can inform a range of strategic decisions.
   - Complexity: JOIN, GROUP BY, CASE, Subquery
8. Description: Identify coaches whose trainees have renewed their memberships at the highest rates, suggesting high coach performance.
      PICTURE
   - Justification: Enables the club to identify and reward top-performing coaches, potentially using this information for marketing or compensation strategies.
   - Complexity: Complex (Join, Subquery, Window Functions)
9. Description: Calculate the total hours worked by each staff member in a given day, including details of their position.
      PICTURE
   - Justification: Provides insights into staff workload distribution, helping to identify under or overutilized staff for better resource management.
   - Complexity: (Join, Date Functions, Aggregate Functions)
10. Description: Calculate the total monthly payment received from all active members.
      PICTURE
   - Justification: Provides a quick overview of the club's primary income source, helping in financial planning.
   - Complexity: Simple (Aggregate Function).
