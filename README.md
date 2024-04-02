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
INSERT
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
   - Complexity: Simple (Aggregate Function)
