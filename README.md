# Police-Station-Administrative-Management-Citizen-Assistance-System
The basic idea behind the program is to reduce the workload of the police force of Pune City. So we developed a system to handle administrative jobs in a police station such as keeping a record of FIRs, previous arrests, criminals in custody, etc. Along with this, the citizen assistance system consisted of online FIR filing and finding the nearest police station.

1. POLICE SUPPORT SYSTEM :-

We first confirm that it’s actually a police official with the help of an authorization
key. If he puts the correct password, he gets the access to do the following
operations :-
1) Edit jail records
2)Edit most wanted criminal list
3) View FIR records
4) View active cases/ displaying investigating FIRs.
5)Update case status

2. CITIZEN SUPPORT SYSTEM:-

Citizens can do the following things:-

a) File an FIR
b) Withdraw FIR
c) Find nearest police station to their current location

GRAPH
1. The graph is used to store different locations of
Pune and roads connecting those locations.
2. We have used Djikstra’s Algorithm to find the
nearest police station from the citizen’s current
location.

HASHTABLE
1. We have used a hashtable to do FIR Manaagement.
2. Generating Hash Key :-
  a) Every FIR has been given a Category Type. And the hash function
uses that category type to generate the Hash Key.
3. So the Hashtable stores FIRs related to specific category of crime
under a specific index.
4. So all crimes of a one particular type remain grouped together.

HEAP
1) We have a list for carrying out Most Wanted Criminal operations
which include adding criminals to the list, removing them from the
list.
2) We have calculated severity of every criminal based on the
crimes they have committed.
3) Based on the basis of the severity value calculated, Max Heap is
generated which gives us the most wanted criminal.
4) Once the criminal has been caught, we are removing them from
our records.

ARRAY
1. We have used an array to carry out operations on the jail
records which include :-
a) Adding criminal to our jail.
b) Displaying jail records
c) Removing from jail records
