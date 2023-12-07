# Document Summary

Upon socialising of this Inventory, and eventual agreement, we will
progress to detailing how the Acceptance will be accomplished and
signoff achieved, the 'Accepted' column will be marked Yes once
consensus is reached.

# Change Management

Upon agreement on the User Story Inventory, a suitable level of Change
Management will be applied, this will enable us to phase-deliver
Governance on Cardano and to fulfil the ongoing Ecosystem and Community
needs. Additional User Stories will be proposed, reviewed, approved and
accepted using

# Source Areas Under Consideration

This section shows the areas or sources thus far

  -------------------------------------------------
  Source       Outline        State      Key
               Contribution              Contract
  ------------ -------------- ---------- ----------
  Voltaire     Use Cases for  Initial    Outreach
               Governance,    Capture    in
               voting,        Complete   progress
               delegation                

  CIP-1694     Blockchain     Initial    Outreach
               level User     Capture    in
               Stories on     Complete   progress
               voting,                   
               delegation,               
               identity,                 
               consensus                 

  Smart        Plutus v3 and  Initial    Outreach
  Contracts    BLS            Capture    in
                              Complete   progress

  CLI-API      Interface      Initial    Outreach
               outline and    Capture    in
               definition     Complete   progress

  Sidechains   Interaction    Outreach   Outreach
               with BLS       in         in
               primitives     progress   progress

  DApps        To be defined  To be      Outreach
               and elaborated defined    in
                                         progress

  Exchanges    To be defined  To be      Outreach
               and elaborated defined    in
                                         progress

  Other        To be defined  To be      Outreach
               and elaborated defined    in
                                         progress
  -------------------------------------------------

# User Story (Voltaire, API, CIP-1694, Community et al)

+------+------+--------------+------------------+---+---+----+------+
| UID  | User | Functional   | Acceptance       | L | A | So | Enab |
|      | S    | Requirement  | Criteria         | i | c | ur | ler( |
|      | tory |              |                  | n | c | ce | Y,N) |
|      |      |              |                  | k | e |    |      |
|      |      |              |                  |   | p |    |      |
|      |      |              |                  |   | t |    |      |
|      |      |              |                  |   | e |    |      |
|      |      |              |                  |   | d |    |      |
+======+======+==============+==================+===+===+====+======+
| CH   | As a | Connect with | Given I am on    |   |   | Vo | N    |
| .VO1 | DRep | multiple     | the homepage     |   |   | lt |      |
|      | or   | stake key    |                  |   |   | ai |      |
|      | Ada  | wallet       | And my wallet is |   |   | re |      |
|      | Ho   |              | not connected.   |   |   |    |      |
|      | lder |              |                  |   |   |    |      |
|      | I    |              | When I click the |   |   |    |      |
|      | want |              | Connect Wallet   |   |   |    |      |
|      | to   |              | button           |   |   |    |      |
|      | con  |              |                  |   |   |    |      |
|      | nect |              | And select (one  |   |   |    |      |
|      | my   |              | of) my CIP-95    |   |   |    |      |
|      | wa   |              | compatible       |   |   |    |      |
|      | llet |              | wallet(s) with   |   |   |    |      |
|      | to   |              | multiple stake   |   |   |    |      |
|      | Gov  |              | keys             |   |   |    |      |
|      | Tool |              |                  |   |   |    |      |
|      | so   |              | And select from  |   |   |    |      |
|      | that |              | a list which     |   |   |    |      |
|      | I    |              | stake key I wish |   |   |    |      |
|      | can  |              | to connect with  |   |   |    |      |
|      | post |              |                  |   |   |    |      |
|      | tran |              | Then the wallet  |   |   |    |      |
|      | sact |              | will prompt me   |   |   |    |      |
|      | ions |              | to connect and I |   |   |    |      |
|      | on-c |              | can connect to   |   |   |    |      |
|      | hain |              | GovTool with it  |   |   |    |      |
|      |      |              | on the selected  |   |   |    |      |
|      |      |              | stake key.       |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given I am on    |   |   | Vo | N    |
|      |      |              | the homepage     |   |   | lt |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              | And my wallet is |   |   | re |      |
|      |      |              | not connected    |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I click the |   |   |    |      |
|      |      |              | Connect Wallet   |   |   |    |      |
|      |      |              | button           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I am not    |   |   |    |      |
|      |      |              | shown any non    |   |   |    |      |
|      |      |              | CIP-95           |   |   |    |      |
|      |      |              | compatible       |   |   |    |      |
|      |      |              | wallets.         |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given I am on    |   |   | Vo | N    |
|      |      |              | the homepage     |   |   | lt |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              | And my wallet is |   |   | re |      |
|      |      |              | not connected    |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I click the |   |   |    |      |
|      |      |              | Connect Wallet   |   |   |    |      |
|      |      |              | button and       |   |   |    |      |
|      |      |              | select a CIP-95  |   |   |    |      |
|      |      |              | compliant,       |   |   |    |      |
|      |      |              | multiple stake   |   |   |    |      |
|      |      |              | key wallet,      |   |   |    |      |
|      |      |              | containing zero  |   |   |    |      |
|      |      |              | ADA (or tADA for |   |   |    |      |
|      |      |              | SanchoNet)       |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then a modal     |   |   |    |      |
|      |      |              | window opens     |   |   |    |      |
|      |      |              | showing my       |   |   |    |      |
|      |      |              | CIP-95           |   |   |    |      |
|      |      |              | compatible       |   |   |    |      |
|      |      |              | wallets          |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I select a  |   |   |    |      |
|      |      |              | wallet with      |   |   |    |      |
|      |      |              | multiple stake   |   |   |    |      |
|      |      |              | keys from this   |   |   |    |      |
|      |      |              | list             |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I am asked  |   |   |    |      |
|      |      |              | which stake key  |   |   |    |      |
|      |      |              | I wish to        |   |   |    |      |
|      |      |              | connect with     |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I select a  |   |   |    |      |
|      |      |              | stake key        |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then the wallet  |   |   |    |      |
|      |      |              | opens and I can  |   |   |    |      |
|      |      |              | connect with it  |   |   |    |      |
|      |      |              | on the selected  |   |   |    |      |
|      |      |              | stake key.       |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given i am on    |   |   | Vo | N    |
|      |      |              | the homepage     |   |   | lt |      |
|      |      |              | without my       |   |   | ai |      |
|      |      |              | wallet connected |   |   | re |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I click the |   |   |    |      |
|      |      |              | Connect Wallet   |   |   |    |      |
|      |      |              | button and       |   |   |    |      |
|      |      |              | select a CIP-95  |   |   |    |      |
|      |      |              | compliant,       |   |   |    |      |
|      |      |              | single stake key |   |   |    |      |
|      |      |              | wallet,          |   |   |    |      |
|      |      |              | containing more  |   |   |    |      |
|      |      |              | than zero ADA    |   |   |    |      |
|      |      |              | (or tADA for     |   |   |    |      |
|      |      |              | SanchoNet)       |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then a modal     |   |   |    |      |
|      |      |              | window opens     |   |   |    |      |
|      |      |              | showing my       |   |   |    |      |
|      |      |              | CIP-95           |   |   |    |      |
|      |      |              | compatible       |   |   |    |      |
|      |      |              | wallets          |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I select a  |   |   |    |      |
|      |      |              | wallet with      |   |   |    |      |
|      |      |              | multiple stake   |   |   |    |      |
|      |      |              | keys from this   |   |   |    |      |
|      |      |              | list             |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I am asked  |   |   |    |      |
|      |      |              | which stake key  |   |   |    |      |
|      |      |              | I wish to        |   |   |    |      |
|      |      |              | connect with     |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I select a  |   |   |    |      |
|      |      |              | stake key        |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then the wallet  |   |   |    |      |
|      |      |              | opens and I can  |   |   |    |      |
|      |      |              | connect with it  |   |   |    |      |
|      |      |              | on the selected  |   |   |    |      |
|      |      |              | stake key.       |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Connect with | Given I am on    |   |   | Vo | N    |
|      |      | single stake | the homepage     |   |   | lt |      |
|      |      | key wallet   | with no wallet   |   |   | ai |      |
|      |      |              | connected        |   |   | re |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I click the |   |   |    |      |
|      |      |              | Connect Wallet   |   |   |    |      |
|      |      |              | button and       |   |   |    |      |
|      |      |              | select a CIP-95  |   |   |    |      |
|      |      |              | compliant single |   |   |    |      |
|      |      |              | stake key wallet |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then my wallet   |   |   |    |      |
|      |      |              | appears and I    |   |   |    |      |
|      |      |              | can connect with |   |   |    |      |
|      |      |              | it               |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given I am on    |   |   | Vo | N    |
|      |      |              | the homepage     |   |   | lt |      |
|      |      |              | without my       |   |   | ai |      |
|      |      |              | wallet connected |   |   | re |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I click the |   |   |    |      |
|      |      |              | Connect Wallet   |   |   |    |      |
|      |      |              | button           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I am not    |   |   |    |      |
|      |      |              | shown any non    |   |   |    |      |
|      |      |              | CIP-95           |   |   |    |      |
|      |      |              | compatible       |   |   |    |      |
|      |      |              | wallets.         |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given I am on    |   |   | Vo | N    |
|      |      |              | the homepage     |   |   | lt |      |
|      |      |              | without my       |   |   | ai |      |
|      |      |              | wallet connected |   |   | re |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I click the |   |   |    |      |
|      |      |              | Connect Wallet   |   |   |    |      |
|      |      |              | button and       |   |   |    |      |
|      |      |              | select a CIP-95  |   |   |    |      |
|      |      |              | compliant,       |   |   |    |      |
|      |      |              | single stake key |   |   |    |      |
|      |      |              | wallet,          |   |   |    |      |
|      |      |              | containing zero  |   |   |    |      |
|      |      |              | ADA (or tADA for |   |   |    |      |
|      |      |              | SanchoNet)       |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then my wallet   |   |   |    |      |
|      |      |              | appears and I    |   |   |    |      |
|      |      |              | can connect with |   |   |    |      |
|      |      |              | it               |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given I am on    |   |   | Vo | N    |
|      |      |              | the homepage     |   |   | lt |      |
|      |      |              | without my       |   |   | ai |      |
|      |      |              | wallet connected |   |   | re |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I click the |   |   |    |      |
|      |      |              | Connect Wallet   |   |   |    |      |
|      |      |              | button and       |   |   |    |      |
|      |      |              | select a CIP-95  |   |   |    |      |
|      |      |              | compliant,       |   |   |    |      |
|      |      |              | single stake key |   |   |    |      |
|      |      |              | wallet,          |   |   |    |      |
|      |      |              | containing more  |   |   |    |      |
|      |      |              | than zero ADA    |   |   |    |      |
|      |      |              | (or tADA for     |   |   |    |      |
|      |      |              | SanchoNet)       |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then my wallet   |   |   |    |      |
|      |      |              | appears and I    |   |   |    |      |
|      |      |              | can connect with |   |   |    |      |
|      |      |              | it               |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Disconnect   | Given that I am  |   |   | Vo | N    |
|      |      | wallet       | on the dashboard |   |   | lt |      |
|      |      |              | with my wallet   |   |   | ai |      |
|      |      |              | connected        |   |   | re |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | If I click the   |   |   |    |      |
|      |      |              | Disconnect       |   |   |    |      |
|      |      |              | button           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then my wallet   |   |   |    |      |
|      |      |              | is disconnected  |   |   |    |      |
|      |      |              | from GovTool and |   |   |    |      |
|      |      |              | I am redirected  |   |   |    |      |
|      |      |              | to the homepage. |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   | Vo | N    |
|      |      |              | connected to     |   |   | lt |      |
|      |      |              | GovTool with my  |   |   | ai |      |
|      |      |              | wallet           |   |   | re |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I           |   |   |    |      |
|      |      |              | disconnect       |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I will be   |   |   |    |      |
|      |      |              | redirected to    |   |   |    |      |
|      |      |              | the homepage,    |   |   |    |      |
|      |      |              | and will not     |   |   |    |      |
|      |      |              | have access to   |   |   |    |      |
|      |      |              | delegation or    |   |   |    |      |
|      |      |              | voting features. |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Check the    | Given I am on    |   |   | Vo | N    |
|      |      | wallet is on | the homepage\    |   |   | lt |      |
|      |      | the correct  | \                |   |   | ai |      |
|      |      | network      | When I compare   |   |   | re |      |
|      |      |              | the networkId    |   |   |    |      |
|      |      |              | with the         |   |   |    |      |
|      |      |              | environment      |   |   |    |      |
|      |      |              | value set on the |   |   |    |      |
|      |      |              | deployment for   |   |   |    |      |
|      |      |              | the network.     |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then if there    |   |   |    |      |
|      |      |              | are exceptions   |   |   |    |      |
|      |      |              | raised, fail the |   |   |    |      |
|      |      |              | test.            |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | If no            |   |   |    |      |
|      |      |              | exceptions,      |   |   |    |      |
|      |      |              | connect the      |   |   |    |      |
|      |      |              | wallet to the    |   |   |    |      |
|      |      |              | network (pass)   |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CH   | As   | Delegate to  | Given that I     |   |   | Vo | N    |
| .VO2 | an   | DRep ID      | have my wallet   |   |   | lt |      |
|      | Ada  |              | connected, and I |   |   | ai |      |
|      | Ho   |              | am on the        |   |   | re |      |
|      | lder |              | Delegate to DRep |   |   |    |      |
|      | I    |              | page             |   |   |    |      |
|      | want |              |                  |   |   |    |      |
|      | to   |              | When I select    |   |   |    |      |
|      | dele |              | the delegate to  |   |   |    |      |
|      | gate |              | DRep ID option   |   |   |    |      |
|      | my   |              | and I enter a    |   |   |    |      |
|      | vo   |              | DRep ID which    |   |   |    |      |
|      | ting |              | has not been     |   |   |    |      |
|      | p    |              | registered and I |   |   |    |      |
|      | ower |              | press delegate   |   |   |    |      |
|      | to a |              |                  |   |   |    |      |
|      | DRep |              | Then I will be   |   |   |    |      |
|      | so   |              | presented with   |   |   |    |      |
|      | that |              | an error message |   |   |    |      |
|      | I    |              | explaining that  |   |   |    |      |
|      | can  |              | the DRep ID was  |   |   |    |      |
|      | c    |              | not found.       |   |   |    |      |
|      | laim |              |                  |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | sta  |              |                  |   |   |    |      |
|      | king |              |                  |   |   |    |      |
|      | rew  |              |                  |   |   |    |      |
|      | ards |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I     |   |   | Vo | N    |
|      |      |              | have my wallet   |   |   | lt |      |
|      |      |              | connected, and I |   |   | ai |      |
|      |      |              | am on the        |   |   | re |      |
|      |      |              | delegate to DRep |   |   |    |      |
|      |      |              | page,            |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I choose    |   |   |    |      |
|      |      |              | the Delegate to  |   |   |    |      |
|      |      |              | DRep ID option   |   |   |    |      |
|      |      |              | and I enter a    |   |   |    |      |
|      |      |              | registered DRep  |   |   |    |      |
|      |      |              | ID and I press   |   |   |    |      |
|      |      |              | the Delegate     |   |   |    |      |
|      |      |              | button           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I am able   |   |   |    |      |
|      |      |              | to delegate to   |   |   |    |      |
|      |      |              | that DRep ID via |   |   |    |      |
|      |      |              | my connected     |   |   |    |      |
|      |      |              | wallet           |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I     |   |   | Vo | N    |
|      |      |              | have connected   |   |   | lt |      |
|      |      |              | to GovTool with  |   |   | ai |      |
|      |      |              | zero\* ADA (or   |   |   | re |      |
|      |      |              | tADA in the case |   |   |    |      |
|      |      |              | of SanchoNet)    |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I choose    |   |   |    |      |
|      |      |              | the Delegate to  |   |   |    |      |
|      |      |              | DRep ID option   |   |   |    |      |
|      |      |              | and I enter a    |   |   |    |      |
|      |      |              | registered DRep  |   |   |    |      |
|      |      |              | ID and I press   |   |   |    |      |
|      |      |              | the Delegate     |   |   |    |      |
|      |      |              | button           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I am        |   |   |    |      |
|      |      |              | presented with a |   |   |    |      |
|      |      |              | warning message  |   |   |    |      |
|      |      |              | and cannot       |   |   |    |      |
|      |      |              | proceed with     |   |   |    |      |
|      |      |              | delegation.      |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | \*or at least a  |   |   |    |      |
|      |      |              | number below     |   |   |    |      |
|      |      |              | transaction      |   |   |    |      |
|      |      |              | costs            |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Access       | Given that I do  |   |   | Vo | N    |
|      |      | Delegate to  | not have a       |   |   | lt |      |
|      |      | DRep page    | compatible       |   |   | ai |      |
|      |      |              | wallet connected |   |   | re |      |
|      |      |              | to GovTool       |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I attempt   |   |   |    |      |
|      |      |              | to visit the URL |   |   |    |      |
|      |      |              | of the Delegate  |   |   |    |      |
|      |      |              | to DRep page     |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I am        |   |   |    |      |
|      |      |              | redirected to    |   |   |    |      |
|      |      |              | the homepage     |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I     |   |   | Vo | N    |
|      |      |              | have a           |   |   | lt |      |
|      |      |              | compatible       |   |   | ai |      |
|      |      |              | wallet connected |   |   | re |      |
|      |      |              | to GovTool and I |   |   |    |      |
|      |      |              | am looking at    |   |   |    |      |
|      |      |              | the dashboard    |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I click on  |   |   |    |      |
|      |      |              | the the Delegate |   |   |    |      |
|      |      |              | button (or       |   |   |    |      |
|      |      |              | Change           |   |   |    |      |
|      |      |              | Delegation       |   |   |    |      |
|      |      |              | button if you    |   |   |    |      |
|      |      |              | are already      |   |   |    |      |
|      |      |              | registered)      |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I am shown  |   |   |    |      |
|      |      |              | the Delegate to  |   |   |    |      |
|      |      |              | DRep page        |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Verify DRep  | Given that I\'m  |   |   | Vo | N    |
|      |      | behaviour in | not connected to |   |   | lt |      |
|      |      | connected    | the wallet       |   |   | ai |      |
|      |      | state        |                  |   |   | re |      |
|      |      |              | When I visit the |   |   |    |      |
|      |      |              | DRep delegation  |   |   |    |      |
|      |      |              | page, and I      |   |   |    |      |
|      |      |              | click the        |   |   |    |      |
|      |      |              | delegate-conne   |   |   |    |      |
|      |      |              | ct-wallet-button |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then the connect |   |   |    |      |
|      |      |              | your             |   |   |    |      |
|      |      |              | wallet-modal is  |   |   |    |      |
|      |      |              | visible          |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Verify DRep  | Given that I     |   |   | Vo | N    |
|      |      | behaviour in | have a preset    |   |   | lt |      |
|      |      | disconnected | dRep wallet      |   |   | ai |      |
|      |      | state        | loaded           |   |   | re |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then Delegate    |   |   |    |      |
|      |      |              | button is        |   |   |    |      |
|      |      |              | clicked          |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then it is       |   |   |    |      |
|      |      |              | expected that    |   |   |    |      |
|      |      |              | delegation       |   |   |    |      |
|      |      |              | options card is  |   |   |    |      |
|      |      |              | visible          |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | delegate to      |   |   |    |      |
|      |      |              | myself is        |   |   |    |      |
|      |      |              | expected to be   |   |   |    |      |
|      |      |              | visible          |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then Other       |   |   |    |      |
|      |      |              | options is       |   |   |    |      |
|      |      |              | clicked          |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Expect that      |   |   |    |      |
|      |      |              | signal no        |   |   |    |      |
|      |      |              | confidence card  |   |   |    |      |
|      |      |              | and vote abstain |   |   |    |      |
|      |      |              | cards are        |   |   |    |      |
|      |      |              | visible          |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Next, delegate   |   |   |    |      |
|      |      |              | to dRep card is  |   |   |    |      |
|      |      |              | clicked,         |   |   |    |      |
|      |      |              | followed by next |   |   |    |      |
|      |      |              | step button      |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then expected    |   |   |    |      |
|      |      |              | that dRep ID     |   |   |    |      |
|      |      |              | input is visible |   |   |    |      |
|      |      |              | along with       |   |   |    |      |
|      |      |              | delegate button  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Delegate to  | Given that I am  |   |   | Vo | N    |
|      |      | myself       | a registered     |   |   | lt |      |
|      |      |              | DRep who is      |   |   | ai |      |
|      |      |              | connected to     |   |   | re |      |
|      |      |              | GovTool with my  |   |   |    |      |
|      |      |              | wallet, and I am |   |   |    |      |
|      |      |              | on the Delegate  |   |   |    |      |
|      |      |              | to DRep page     |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I choose    |   |   |    |      |
|      |      |              | the Delegate to  |   |   |    |      |
|      |      |              | DRep ID option   |   |   |    |      |
|      |      |              | and I enter my   |   |   |    |      |
|      |      |              | own DRep ID and  |   |   |    |      |
|      |      |              | I press the      |   |   |    |      |
|      |      |              | Delegate button  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I am able   |   |   |    |      |
|      |      |              | to delegate to   |   |   |    |      |
|      |      |              | myself via my    |   |   |    |      |
|      |      |              | connected wallet |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   | Vo | N    |
|      |      |              | a registered     |   |   | lt |      |
|      |      |              | DRep who is      |   |   | ai |      |
|      |      |              | connected to     |   |   | re |      |
|      |      |              | GovTool with my  |   |   |    |      |
|      |      |              | wallet, and I am |   |   |    |      |
|      |      |              | on the Delegate  |   |   |    |      |
|      |      |              | to DRep page     |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I select    |   |   |    |      |
|      |      |              | the Delegate to  |   |   |    |      |
|      |      |              | Myself option    |   |   |    |      |
|      |      |              | and press the    |   |   |    |      |
|      |      |              | Delegate button  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I will be   |   |   |    |      |
|      |      |              | able to send a   |   |   |    |      |
|      |      |              | transaction to   |   |   |    |      |
|      |      |              | delegate to      |   |   |    |      |
|      |      |              | myself via my    |   |   |    |      |
|      |      |              | wallet           |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   | Vo | N    |
|      |      |              | not a registered |   |   | lt |      |
|      |      |              | DRep, and I am   |   |   | ai |      |
|      |      |              | connected to     |   |   | re |      |
|      |      |              | GovTool with my  |   |   |    |      |
|      |      |              | wallet,          |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I am on the |   |   |    |      |
|      |      |              | Delegate to DRep |   |   |    |      |
|      |      |              | page             |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | I cannot see a   |   |   |    |      |
|      |      |              | Delegate to      |   |   |    |      |
|      |      |              | Myself option    |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Change my    | Given that I am  |   |   | Vo | N    |
|      |      | DRep         | I am already     |   |   | lt |      |
|      |      | delegation   | delegated to a   |   |   | ai |      |
|      |      |              | DRep             |   |   | re |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I look at   |   |   |    |      |
|      |      |              | the dashboard    |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | GovTool will     |   |   |    |      |
|      |      |              | know that I am   |   |   |    |      |
|      |      |              | delegated and    |   |   |    |      |
|      |      |              | will invite me   |   |   |    |      |
|      |      |              | to "change my    |   |   |    |      |
|      |      |              | delegation"      |   |   |    |      |
|      |      |              | rather than to   |   |   |    |      |
|      |      |              | delegate.        |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   | Vo | N    |
|      |      |              | already          |   |   | lt |      |
|      |      |              | delegated        |   |   | ai |      |
|      |      |              |                  |   |   | re |      |
|      |      |              | When I go to     |   |   |    |      |
|      |      |              | change my        |   |   |    |      |
|      |      |              | delegation       |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | I can delegate   |   |   |    |      |
|      |      |              | to any           |   |   |    |      |
|      |      |              | registered DRep, |   |   |    |      |
|      |      |              | If I am          |   |   |    |      |
|      |      |              | delegated to     |   |   |    |      |
|      |      |              | myself then the  |   |   |    |      |
|      |      |              | option to        |   |   |    |      |
|      |      |              | "delegate to     |   |   |    |      |
|      |      |              | myself" will not |   |   |    |      |
|      |      |              | be shown, If I   |   |   |    |      |
|      |      |              | am delegated to  |   |   |    |      |
|      |      |              | a specific       |   |   |    |      |
|      |      |              | predefined DRep  |   |   |    |      |
|      |      |              | then this        |   |   |    |      |
|      |      |              | predefined       |   |   |    |      |
|      |      |              | option will not  |   |   |    |      |
|      |      |              | be shown.        |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Check the    | Given that I     |   |   | Vo | N    |
|      |      | validity of  | have selected    |   |   | lt |      |
|      |      | a DRep ID    | the "delegate to |   |   | ai |      |
|      |      |              | a DRep ID"       |   |   | re |      |
|      |      |              | option in the    |   |   |    |      |
|      |      |              | delegation user  |   |   |    |      |
|      |      |              | journey.\        |   |   |    |      |
|      |      |              | \                |   |   |    |      |
|      |      |              | When I enter     |   |   |    |      |
|      |      |              | anything in the  |   |   |    |      |
|      |      |              | DRep ID input    |   |   |    |      |
|      |      |              | box that is not  |   |   |    |      |
|      |      |              | a registered     |   |   |    |      |
|      |      |              | DRep ID.\        |   |   |    |      |
|      |      |              | \                |   |   |    |      |
|      |      |              | Then I will not  |   |   |    |      |
|      |      |              | be able to       |   |   |    |      |
|      |      |              | delegate to this |   |   |    |      |
|      |      |              | DRep ID and will |   |   |    |      |
|      |      |              | get a warning    |   |   |    |      |
|      |      |              | message.         |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Delegate to  | Given that I am  |   |   | Vo |      |
|      |      | Abstain      | a DRep           |   |   | lt |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              | When I delegate  |   |   | re |      |
|      |      |              | using the        |   |   |    |      |
|      |      |              | "delegate to     |   |   |    |      |
|      |      |              | abstain" feature |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then it will     |   |   |    |      |
|      |      |              | only delegate my |   |   |    |      |
|      |      |              | own lovelace's   |   |   |    |      |
|      |      |              | voting power to  |   |   |    |      |
|      |      |              | Abstain and NOT  |   |   |    |      |
|      |      |              | the voting power |   |   |    |      |
|      |      |              | (if any) that    |   |   |    |      |
|      |      |              | has been         |   |   |    |      |
|      |      |              | delegated to me  |   |   |    |      |
|      |      |              | by others. I     |   |   |    |      |
|      |      |              | will be notified |   |   |    |      |
|      |      |              | that my          |   |   |    |      |
|      |      |              | delegation       |   |   |    |      |
|      |      |              | translation was  |   |   |    |      |
|      |      |              | sent.            |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   |    |      |
|      |      |              | not a DRep       |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I delegate  |   |   |    |      |
|      |      |              | using the        |   |   |    |      |
|      |      |              | "delegate to     |   |   |    |      |
|      |      |              | abstain" feature |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then it will     |   |   |    |      |
|      |      |              | delegate any     |   |   |    |      |
|      |      |              | voting power I   |   |   |    |      |
|      |      |              | have to Abstain. |   |   |    |      |
|      |      |              | I will be        |   |   |    |      |
|      |      |              | notified that my |   |   |    |      |
|      |      |              | delegation       |   |   |    |      |
|      |      |              | translation was  |   |   |    |      |
|      |      |              | sent.            |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Delegate to  | Given that I am  |   |   | Vo |      |
|      |      | N            | a DRep           |   |   | lt |      |
|      |      | o-Confidence |                  |   |   | ai |      |
|      |      |              | When I delegate  |   |   | re |      |
|      |      |              | using the        |   |   |    |      |
|      |      |              | "delegate to     |   |   |    |      |
|      |      |              | no-confidence"   |   |   |    |      |
|      |      |              | feature          |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then it will     |   |   |    |      |
|      |      |              | only delegate my |   |   |    |      |
|      |      |              | own lovelace's   |   |   |    |      |
|      |      |              | voting power to  |   |   |    |      |
|      |      |              | No-Confidence    |   |   |    |      |
|      |      |              | and NOT the      |   |   |    |      |
|      |      |              | voting power (if |   |   |    |      |
|      |      |              | any) that has    |   |   |    |      |
|      |      |              | been delegated   |   |   |    |      |
|      |      |              | to me by others. |   |   |    |      |
|      |      |              | I will be        |   |   |    |      |
|      |      |              | notified that my |   |   |    |      |
|      |      |              | delegation       |   |   |    |      |
|      |      |              | translation was  |   |   |    |      |
|      |      |              | sent.            |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   | Vo |      |
|      |      |              | not a DRep       |   |   | lt |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              | When I delegate  |   |   | re |      |
|      |      |              | using the        |   |   |    |      |
|      |      |              | "delegate to     |   |   |    |      |
|      |      |              | no-confidence"   |   |   |    |      |
|      |      |              | feature          |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then it will     |   |   |    |      |
|      |      |              | delegate any     |   |   |    |      |
|      |      |              | voting power I   |   |   |    |      |
|      |      |              | have to          |   |   |    |      |
|      |      |              | No-Confi. I will |   |   |    |      |
|      |      |              | be notified that |   |   |    |      |
|      |      |              | my delegation    |   |   |    |      |
|      |      |              | translation was  |   |   |    |      |
|      |      |              | sent.            |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Guardrails   | This work is in  |   |   | Vo |      |
|      |      | for Voltaire | progress         |   |   | lt |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | re |      |
+------+------+--------------+------------------+---+---+----+------+
| CH   | As a | Register as  | Given that I am  |   |   | Vo | N    |
| .VO3 | DRep | a DRep       | connected to     |   |   | lt |      |
|      | I    |              | GovTool with a   |   |   | ai |      |
|      | want |              | compatible       |   |   | re |      |
|      | to   |              | wallet           |   |   |    |      |
|      | regi |              |                  |   |   |    |      |
|      | ster |              | When I go        |   |   |    |      |
|      | so   |              | through the DRep |   |   |    |      |
|      | that |              | registration     |   |   |    |      |
|      | I    |              | process, and do  |   |   |    |      |
|      | can  |              | not include a    |   |   |    |      |
|      | vote |              | metadata anchor  |   |   |    |      |
|      | on   |              |                  |   |   |    |      |
|      | go   |              | Then I can       |   |   |    |      |
|      | vern |              | register as a    |   |   |    |      |
|      | ance |              | DRep via my      |   |   |    |      |
|      | act  |              | wallet (because  |   |   |    |      |
|      | ions |              | metadata anchors |   |   |    |      |
|      |      |              | are optional)    |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   | Vo | N    |
|      |      |              | connected to     |   |   | lt |      |
|      |      |              | GovTool with a   |   |   | ai |      |
|      |      |              | compatible       |   |   | re |      |
|      |      |              | wallet           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I go        |   |   |    |      |
|      |      |              | through the DRep |   |   |    |      |
|      |      |              | registration     |   |   |    |      |
|      |      |              | process, and     |   |   |    |      |
|      |      |              | include metadata |   |   |    |      |
|      |      |              | anchor           |   |   |    |      |
|      |      |              | information in   |   |   |    |      |
|      |      |              | the wrong format |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I will not  |   |   |    |      |
|      |      |              | be able to       |   |   |    |      |
|      |      |              | progress further |   |   |    |      |
|      |      |              | in the process   |   |   |    |      |
|      |      |              | and I will be    |   |   |    |      |
|      |      |              | told that it is  |   |   |    |      |
|      |      |              | because the      |   |   |    |      |
|      |      |              | format is        |   |   |    |      |
|      |      |              | incorrect.       |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   | Vo | N    |
|      |      |              | connected to     |   |   | lt |      |
|      |      |              | GovTool with a   |   |   | ai |      |
|      |      |              | compatible       |   |   | re |      |
|      |      |              | wallet           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I go        |   |   |    |      |
|      |      |              | through the DRep |   |   |    |      |
|      |      |              | registration     |   |   |    |      |
|      |      |              | process, and     |   |   |    |      |
|      |      |              | include metadata |   |   |    |      |
|      |      |              | anchor           |   |   |    |      |
|      |      |              | information in   |   |   |    |      |
|      |      |              | the correct      |   |   |    |      |
|      |      |              | format           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I will be   |   |   |    |      |
|      |      |              | able to register |   |   |    |      |
|      |      |              | as a DRep via my |   |   |    |      |
|      |      |              | wallet, GovTool  |   |   |    |      |
|      |      |              | will include the |   |   |    |      |
|      |      |              | metadata anchor  |   |   |    |      |
|      |      |              | in the           |   |   |    |      |
|      |      |              | registration     |   |   |    |      |
|      |      |              | certificate      |   |   |    |      |
|      |      |              | transaction.     |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Confirm      | Given that I     |   |   | Vo | N    |
|      |      | transaction  | have gone        |   |   | lt |      |
|      |      | has been     | through the DRep |   |   | ai |      |
|      |      | sent         | registration     |   |   | re |      |
|      |      |              | process          |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I press the |   |   |    |      |
|      |      |              | button on my     |   |   |    |      |
|      |      |              | wallet to submit |   |   |    |      |
|      |      |              | the transaction  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I will      |   |   |    |      |
|      |      |              | receive a        |   |   |    |      |
|      |      |              | confirmation     |   |   |    |      |
|      |      |              | message from     |   |   |    |      |
|      |      |              | GovTool that     |   |   |    |      |
|      |      |              | will include a   |   |   |    |      |
|      |      |              | link to the      |   |   |    |      |
|      |      |              | transaction in a |   |   |    |      |
|      |      |              | block explorer.  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Status of    | Given that I     |   |   | Vo | N    |
|      |      | transaction  | have just        |   |   | lt |      |
|      |      | is displayed | submitted a DRep |   |   | ai |      |
|      |      |              | registration     |   |   | re |      |
|      |      |              | transaction, and |   |   |    |      |
|      |      |              | I am looking at  |   |   |    |      |
|      |      |              | the dashboard    |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When the         |   |   |    |      |
|      |      |              | registration has |   |   |    |      |
|      |      |              | not yet been     |   |   |    |      |
|      |      |              | confirmed by the |   |   |    |      |
|      |      |              | blockchain,      |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then the         |   |   |    |      |
|      |      |              | registration     |   |   |    |      |
|      |      |              | status will show |   |   |    |      |
|      |      |              | as "In Progress" |   |   |    |      |
|      |      |              | until it is      |   |   |    |      |
|      |      |              | confirmed.       |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CH   | As a | Should be    | Given that I am  |   |   | Vo | N    |
| .VO4 | DRep | able to      | a DRep and I am  |   |   | lt |      |
|      | I    | access the   | connected to     |   |   | ai |      |
|      | want | governance   | GovTool          |   |   | re |      |
|      | to   | actions page |                  |   |   |    |      |
|      | vote | as a DRep    | When I visit the |   |   |    |      |
|      | so   | with my      | url of the       |   |   |    |      |
|      | that | wallet       | governance       |   |   |    |      |
|      | I    | connected    | actions page     |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | fu   |              | Then the         |   |   |    |      |
|      | lfil |              | governance       |   |   |    |      |
|      | my   |              | actions page is  |   |   |    |      |
|      | role |              | displayed        |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   |    |      |
|      |      |              | a DRep and       |   |   |    |      |
|      |      |              | connected to     |   |   |    |      |
|      |      |              | GovTool          |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I look at   |   |   |    |      |
|      |      |              | the governance   |   |   |    |      |
|      |      |              | actions page     |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then my voting   |   |   |    |      |
|      |      |              | power is         |   |   |    |      |
|      |      |              | displayed        |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   |    |      |
|      |      |              | a DRep and       |   |   |    |      |
|      |      |              | Connected to     |   |   |    |      |
|      |      |              | GovTool, and I   |   |   |    |      |
|      |      |              | am on the        |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | actions page     |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I click     |   |   |    |      |
|      |      |              | Disconnect       |   |   |    |      |
|      |      |              | Wallet           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then my wallet   |   |   |    |      |
|      |      |              | is disconnected  |   |   |    |      |
|      |      |              | and I am         |   |   |    |      |
|      |      |              | redirected to    |   |   |    |      |
|      |      |              | the same page,   |   |   |    |      |
|      |      |              | but without the  |   |   |    |      |
|      |      |              | DRep             |   |   |    |      |
|      |      |              | functionality    |   |   |    |      |
|      |      |              | (i.e. ability to |   |   |    |      |
|      |      |              | vote)            |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   |    |      |
|      |      |              | a DRep and I am  |   |   |    |      |
|      |      |              | on the           |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | actions page     |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I click on  |   |   |    |      |
|      |      |              | the "view        |   |   |    |      |
|      |      |              | proposal         |   |   |    |      |
|      |      |              | details" button  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I will be   |   |   |    |      |
|      |      |              | shown the page   |   |   |    |      |
|      |      |              | for that         |   |   |    |      |
|      |      |              | individual       |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action and be    |   |   |    |      |
|      |      |              | able to view its |   |   |    |      |
|      |      |              | details          |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | A DRep       | Given that I am  |   |   | Vo | N    |
|      |      | should be    | a DRep           |   |   | lt |      |
|      |      | able to vote |                  |   |   | ai |      |
|      |      | on a live    | When I look at   |   |   | re |      |
|      |      | governance   | the details page |   |   |    |      |
|      |      | action       | of an individual |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I can see   |   |   |    |      |
|      |      |              | how many votes   |   |   |    |      |
|      |      |              | the governance   |   |   |    |      |
|      |      |              | action currently |   |   |    |      |
|      |      |              | has for, against |   |   |    |      |
|      |      |              | and abstaining.  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   |    |      |
|      |      |              | a DRep           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I look at   |   |   |    |      |
|      |      |              | the details page |   |   |    |      |
|      |      |              | of an individual |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then there are   |   |   |    |      |
|      |      |              | buttons allowing |   |   |    |      |
|      |      |              | me to vote for,  |   |   |    |      |
|      |      |              | against or       |   |   |    |      |
|      |      |              | abstain.         |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   |    |      |
|      |      |              | a DRep, on the   |   |   |    |      |
|      |      |              | details page of  |   |   |    |      |
|      |      |              | an individual    |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I select    |   |   |    |      |
|      |      |              | yes/ no/         |   |   |    |      |
|      |      |              | abstain, and     |   |   |    |      |
|      |      |              | click vote       |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I can sign  |   |   |    |      |
|      |      |              | & submit this    |   |   |    |      |
|      |      |              | vote via my      |   |   |    |      |
|      |      |              | wallet           |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   |    |      |
|      |      |              | a DRep           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I have      |   |   |    |      |
|      |      |              | submitted a vote |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then Immediately |   |   |    |      |
|      |      |              | after this       |   |   |    |      |
|      |      |              | GovTool will     |   |   |    |      |
|      |      |              | display a        |   |   |    |      |
|      |      |              | message          |   |   |    |      |
|      |      |              | informing me     |   |   |    |      |
|      |      |              | that my          |   |   |    |      |
|      |      |              | transaction has  |   |   |    |      |
|      |      |              | been sent and    |   |   |    |      |
|      |      |              | providing me     |   |   |    |      |
|      |      |              | with a link to a |   |   |    |      |
|      |      |              | block explorer   |   |   |    |      |
|      |      |              | where I can view |   |   |    |      |
|      |      |              | the transaction  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | People       | Given I have     |   |   | Vo | N    |
|      |      | without the  | less Lovelace in |   |   | lt |      |
|      |      | (t)ADA       | my wallet than a |   |   | ai |      |
|      |      | needed to    | transaction      |   |   | re |      |
|      |      | pay for      | costs            |   |   |    |      |
|      |      | voting       |                  |   |   |    |      |
|      |      | transactions | When I attempt   |   |   |    |      |
|      |      | should not   | to vote          |   |   |    |      |
|      |      | be able to   |                  |   |   |    |      |
|      |      | submit a     | The GovTool will |   |   |    |      |
|      |      | voting       | tell me that     |   |   |    |      |
|      |      | transaction  | there is an      |   |   |    |      |
|      |      |              | error            |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | People       | Given that I do  |   |   | Vo | N    |
|      |      | without      | not have a       |   |   | lt |      |
|      |      | their wallet | wallet connected |   |   | ai |      |
|      |      | connected or | to GovTool       |   |   | re |      |
|      |      | who do have  |                  |   |   |    |      |
|      |      | their wallet | When I visit the |   |   |    |      |
|      |      | connected    | details of a     |   |   |    |      |
|      |      | but have not | governance       |   |   |    |      |
|      |      | registered   | action           |   |   |    |      |
|      |      | as DReps     |                  |   |   |    |      |
|      |      | should not   | Then I am not    |   |   |    |      |
|      |      | be able to   | shown a vote     |   |   |    |      |
|      |      | vote         | button.          |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | No one       | Given that I am  |   |   | Vo | N    |
|      |      | should be    | on the           |   |   | lt |      |
|      |      | able to vote | governance       |   |   | ai |      |
|      |      | on a         | action page      |   |   | re |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action that  | When I examine   |   |   |    |      |
|      |      | has expired, | the governance   |   |   |    |      |
|      |      | or been      | actions          |   |   |    |      |
|      |      | ratified, or |                  |   |   |    |      |
|      |      | enacted.     | None of the      |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | actions shown on |   |   |    |      |
|      |      |              | the page have    |   |   |    |      |
|      |      |              | expired or been  |   |   |    |      |
|      |      |              | ratified or      |   |   |    |      |
|      |      |              | enacted.         |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | A DRep       | Given that I am  |   |   | Vo | N    |
|      |      | should be    | a DRep and I     |   |   | lt |      |
|      |      | able to      | have already     |   |   | ai |      |
|      |      | change their | voted on a given |   |   | re |      |
|      |      | vote         | governance       |   |   |    |      |
|      |      |              | action           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I submit a  |   |   |    |      |
|      |      |              | different vote   |   |   |    |      |
|      |      |              | for the same     |   |   |    |      |
|      |      |              | transaction      |   |   |    |      |
|      |      |              | within the same  |   |   |    |      |
|      |      |              | snapshot         |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then the most    |   |   |    |      |
|      |      |              | recent vote will |   |   |    |      |
|      |      |              | be counted.      |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I     |   |   |    | N    |
|      |      |              | have already     |   |   |    |      |
|      |      |              | cast a vote on a |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I examine   |   |   |    |      |
|      |      |              | this specific    |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action's page    |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I can see   |   |   |    |      |
|      |      |              | that I have      |   |   |    |      |
|      |      |              | already voted    |   |   |    |      |
|      |      |              | and what my most |   |   |    |      |
|      |      |              | recent vote was  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I     |   |   | Vo | N    |
|      |      |              | have already     |   |   | lt |      |
|      |      |              | cast a vote on a |   |   | ai |      |
|      |      |              | given governance |   |   | re |      |
|      |      |              | action           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I examine   |   |   |    |      |
|      |      |              | this specific    |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action's page    |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then instead of  |   |   |    |      |
|      |      |              | seeing a "vote"  |   |   |    |      |
|      |      |              | button I should  |   |   |    |      |
|      |      |              | see a "change    |   |   |    |      |
|      |      |              | vote" button     |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Only the     | Given that I am  |   |   | Vo | N    |
|      |      | votes of     | a DRep and I     |   |   | lt |      |
|      |      | participants | vote yes or      |   |   | ai |      |
|      |      | who are      | abstain on a     |   |   | re |      |
|      |      | still DReps  | live governance  |   |   |    |      |
|      |      | at the       | action.          |   |   |    |      |
|      |      | relevant     |                  |   |   |    |      |
|      |      | epoch        | At the epoch     |   |   |    |      |
|      |      | boundary     | boundary         |   |   |    |      |
|      |      | will be      |                  |   |   |    |      |
|      |      | accepted     | My votes are     |   |   |    |      |
|      |      |              | counted.         |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I was |   |   | Vo | N    |
|      |      |              | a DRep that      |   |   | lt |      |
|      |      |              | voted yes or     |   |   | ai |      |
|      |      |              | abstain on a     |   |   | re |      |
|      |      |              | live governance  |   |   |    |      |
|      |      |              | action but then  |   |   |    |      |
|      |      |              | retired.         |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | At the next      |   |   |    |      |
|      |      |              | epoch boundary   |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | My votes will    |   |   |    |      |
|      |      |              | not be counted   |   |   |    |      |
|      |      |              | towards the      |   |   |    |      |
|      |      |              | total tally of   |   |   |    |      |
|      |      |              | DRep votes.      |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | DReps can    | Given that I     |   |   | Vo | N    |
|      |      | attach a     | have chosen how  |   |   | lt |      |
|      |      | metadata     | to vote on the   |   |   | ai |      |
|      |      | anchor to    | UI of a          |   |   | re |      |
|      |      | their votes  | governance       |   |   |    |      |
|      |      |              | action's details |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I add a     |   |   |    |      |
|      |      |              | metadata anchor  |   |   |    |      |
|      |      |              | to the UI also   |   |   |    |      |
|      |      |              | and click the    |   |   |    |      |
|      |      |              | vote button      |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then the         |   |   |    |      |
|      |      |              | resulting        |   |   |    |      |
|      |      |              | transaction will |   |   |    |      |
|      |      |              | include my       |   |   |    |      |
|      |      |              | metadata anchor  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CH   | As a | Only a user  | Given that I am  |   |   | Vo | N    |
| .VO5 | DRep | who is       | not registered   |   |   | lt |      |
|      | I    | registered   | as a DRep,       |   |   | ai |      |
|      | want | as a DRep    |                  |   |   | re |      |
|      | to   | can retire   | When I look for  |   |   |    |      |
|      | re   |              | a retirement     |   |   |    |      |
|      | tire |              | option in        |   |   |    |      |
|      | so   |              | GovTool          |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              | Then there is    |   |   |    |      |
|      | can  |              | none.            |   |   |    |      |
|      | rec  |              |                  |   |   |    |      |
|      | laim |              |                  |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | DRep |              |                  |   |   |    |      |
|      | Dep  |              |                  |   |   |    |      |
|      | osit |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   |    |      |
|      |      |              | registered as a  |   |   |    |      |
|      |      |              | DRep,            |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I look for  |   |   |    |      |
|      |      |              | a retirement     |   |   |    |      |
|      |      |              | option in        |   |   |    |      |
|      |      |              | GovTool there is |   |   |    |      |
|      |      |              | one. And when I  |   |   |    |      |
|      |      |              | choose this      |   |   |    |      |
|      |      |              | option           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then my wallet   |   |   |    |      |
|      |      |              | opens and I can  |   |   |    |      |
|      |      |              | sign a           |   |   |    |      |
|      |      |              | retirement       |   |   |    |      |
|      |      |              | action which is  |   |   |    |      |
|      |      |              | registered       |   |   |    |      |
|      |      |              | on-chain.        |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | When I       | Given that I am  |   |   |    | N    |
|      |      | retire I get | a DRep           |   |   |    |      |
|      |      | my deposit   |                  |   |   |    |      |
|      |      | back         | When I register  |   |   |    |      |
|      |      |              | a valid          |   |   |    |      |
|      |      |              | retirement       |   |   |    |      |
|      |      |              | transaction on   |   |   |    |      |
|      |      |              | chain            |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | then my DRep     |   |   |    |      |
|      |      |              | registration     |   |   |    |      |
|      |      |              | deposit will be  |   |   |    |      |
|      |      |              | returned to me.  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Only a user  | Given that I am  |   |   | Vo | N    |
|      |      | who has the  | not connected to |   |   | lt |      |
|      |      | wallet that  | GovTool          |   |   | ai |      |
|      |      | they         |                  |   |   | re |      |
|      |      | registered   | When I look at   |   |   |    |      |
|      |      | as a DRep    | the homepage     |   |   |    |      |
|      |      | with can     |                  |   |   |    |      |
|      |      | retire.      | Then I will not  |   |   |    |      |
|      |      |              | see an option to |   |   |    |      |
|      |      |              | retire           |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   | Vo | N    |
|      |      |              | connected to     |   |   | lt |      |
|      |      |              | GovTool with an  |   |   | ai |      |
|      |      |              | account that is  |   |   | re |      |
|      |      |              | not associated   |   |   |    |      |
|      |      |              | with a           |   |   |    |      |
|      |      |              | registered DRep  |   |   |    |      |
|      |      |              | certificate      |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I look at   |   |   |    |      |
|      |      |              | the homepage     |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I see an    |   |   |    |      |
|      |      |              | option to        |   |   |    |      |
|      |      |              | register as a    |   |   |    |      |
|      |      |              | DRep             |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   | Vo | N    |
|      |      |              | a registered     |   |   | lt |      |
|      |      |              | DRep with my     |   |   | ai |      |
|      |      |              | wallet account   |   |   | re |      |
|      |      |              | connected        |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I click the |   |   |    |      |
|      |      |              | retire as a DRep |   |   |    |      |
|      |      |              | option on the    |   |   |    |      |
|      |      |              | homepage and     |   |   |    |      |
|      |      |              | then send the    |   |   |    |      |
|      |      |              | retirement       |   |   |    |      |
|      |      |              | transaction with |   |   |    |      |
|      |      |              | my wallet        |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then the         |   |   |    |      |
|      |      |              | blockchain will  |   |   |    |      |
|      |      |              | register my      |   |   |    |      |
|      |      |              | retirement       |   |   |    |      |
|      |      |              | certificate, and |   |   |    |      |
|      |      |              | I will be        |   |   |    |      |
|      |      |              | retired.         |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CH   | As a | A DRep can   | Given that I am  |   |   | Vo | N    |
| .VO6 | DRep | update their | a DRep and am    |   |   | lt |      |
|      | I    | registration | connected to     |   |   | ai |      |
|      | want | after        | GovTool and am   |   |   | re |      |
|      | to   | registering  | on the           |   |   |    |      |
|      | up   |              | dashboard.       |   |   |    |      |
|      | date |              |                  |   |   |    |      |
|      | my   |              | Then when I      |   |   |    |      |
|      | det  |              | click the        |   |   |    |      |
|      | ails |              | "change          |   |   |    |      |
|      | so   |              | metadata" button |   |   |    |      |
|      | that |              | on the DRep tab. |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              | Then I am        |   |   |    |      |
|      | be   |              | directed to      |   |   |    |      |
|      | tter |              | update my        |   |   |    |      |
|      | a    |              | metadata and can |   |   |    |      |
|      | dver |              | submit a DRep    |   |   |    |      |
|      | tise |              | update           |   |   |    |      |
|      | my   |              | certificate to   |   |   |    |      |
|      | self |              | register this    |   |   |    |      |
|      | to   |              | on-chain.        |   |   |    |      |
|      | Ada  |              |                  |   |   |    |      |
|      | Hol  |              |                  |   |   |    |      |
|      | ders |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CH   | As   | Anyone       | Given that I am  |   |   | Vo | N    |
| .VO7 | any  | should be    | on the GovTool   |   |   | lt |      |
|      | user | able to      | homepage,        |   |   | ai |      |
|      | I    | access the   |                  |   |   | re |      |
|      | want | governance   | When I click the |   |   |    |      |
|      | to   | actions page | "Governance      |   |   |    |      |
|      | view | without a    | actions" in the  |   |   |    |      |
|      | go   | wallet       | topbar           |   |   |    |      |
|      | vern | connected    |                  |   |   |    |      |
|      | ance |              | Then I am sent   |   |   |    |      |
|      | act  |              | to the           |   |   |    |      |
|      | ions |              | governance       |   |   |    |      |
|      | so I |              | actions page.    |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | see  |              |                  |   |   |    |      |
|      | what |              |                  |   |   |    |      |
|      | is   |              |                  |   |   |    |      |
|      | b    |              |                  |   |   |    |      |
|      | eing |              |                  |   |   |    |      |
|      | prop |              |                  |   |   |    |      |
|      | osed |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | I can see    | Given that I am  |   |   | Vo | N    |
|      |      | all live     | on the           |   |   | lt |      |
|      |      | governance   | Governance       |   |   | ai |      |
|      |      | actions      | Actions page     |   |   | re |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | When I review    |   |   |    |      |
|      |      |              | the governance   |   |   |    |      |
|      |      |              | actions          |   |   |    |      |
|      |      |              | available to     |   |   |    |      |
|      |      |              | view on the      |   |   |    |      |
|      |      |              | page,            |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then all of the  |   |   |    |      |
|      |      |              | non expired/     |   |   |    |      |
|      |      |              | ratified/enacted |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | actions.         |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Anyone with  | Given that I am  |   |   | Vo | N    |
|      |      | a CIP-95     | on the GovTool   |   |   | lt |      |
|      |      | compatible   | dashboard,       |   |   | ai |      |
|      |      | wallet       |                  |   |   | re |      |
|      |      | connected    | When I click the |   |   |    |      |
|      |      | should be    | View Governance  |   |   |    |      |
|      |      | able to      | Actions tab, or  |   |   |    |      |
|      |      | access the   | "Governance      |   |   |    |      |
|      |      | governance   | actions" in the  |   |   |    |      |
|      |      | actions page | sidebar          |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I am sent   |   |   |    |      |
|      |      |              | to the           |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | actions page.    |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Should be    | Given that I am  |   |   | Vo | N    |
|      |      | able to see  | looking at an    |   |   | lt |      |
|      |      | if a         | individual       |   |   | ai |      |
|      |      | governance   | governance       |   |   | re |      |
|      |      | action has   | action,          |   |   |    |      |
|      |      | been         |                  |   |   |    |      |
|      |      | accepted or  | When I look at   |   |   |    |      |
|      |      | rejected by  | how many votes   |   |   |    |      |
|      |      | the          | it has,          |   |   |    |      |
|      |      | Co           |                  |   |   |    |      |
|      |      | nstitutional | Then it shows    |   |   |    |      |
|      |      | Committee    | the number of CC |   |   |    |      |
|      |      |              | votes and        |   |   |    |      |
|      |      |              | whether this is  |   |   |    |      |
|      |      |              | acceptance/veto  |   |   |    |      |
|      |      |              | or neither.      |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Should be    | Given that I am  |   |   | Vo | N    |
|      |      | able to view | looking at a     |   |   | lt |      |
|      |      | relevant     | Treasury         |   |   | ai |      |
|      |      | information  | Withdrawal       |   |   | re |      |
|      |      | about        | governance       |   |   |    |      |
|      |      | governance   | action           |   |   |    |      |
|      |      | actions      |                  |   |   |    |      |
|      |      |              | Then I can see   |   |   |    |      |
|      |      |              | the amount of    |   |   |    |      |
|      |      |              | ADA that the     |   |   |    |      |
|      |      |              | proposal         |   |   |    |      |
|      |      |              | submitter wants  |   |   |    |      |
|      |      |              | to withdraw, and |   |   |    |      |
|      |      |              | the address that |   |   |    |      |
|      |      |              | they want to     |   |   |    |      |
|      |      |              | withdraw it to.  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   |    |      |
|      |      |              | looking at a     |   |   |    |      |
|      |      |              | Proposal         |   |   |    |      |
|      |      |              | Parameter Change |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action,          |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I can see   |   |   |    |      |
|      |      |              | the parameter(s) |   |   |    |      |
|      |      |              | that the         |   |   |    |      |
|      |      |              | Proposal         |   |   |    |      |
|      |      |              | Submitter is     |   |   |    |      |
|      |      |              | proposing to     |   |   |    |      |
|      |      |              | change along     |   |   |    |      |
|      |      |              | with what the    |   |   |    |      |
|      |      |              | current values   |   |   |    |      |
|      |      |              | are, and what he |   |   |    |      |
|      |      |              | wants to change  |   |   |    |      |
|      |      |              | them to.         |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   |    |      |
|      |      |              | looking at a     |   |   |    |      |
|      |      |              | Constitutional   |   |   |    |      |
|      |      |              | Committee Update |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action,          |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I can see   |   |   |    |      |
|      |      |              | the following    |   |   |    |      |
|      |      |              | (where           |   |   |    |      |
|      |      |              | applicable):\    |   |   |    |      |
|      |      |              | - Old Committee  |   |   |    |      |
|      |      |              | Member Cold Key  |   |   |    |      |
|      |      |              | Hash to be       |   |   |    |      |
|      |      |              | removed\         |   |   |    |      |
|      |      |              | - Float, (a      |   |   |    |      |
|      |      |              | rational number  |   |   |    |      |
|      |      |              | in the range     |   |   |    |      |
|      |      |              | from 0 to 1      |   |   |    |      |
|      |      |              | inclusive. Of    |   |   |    |      |
|      |      |              | course if all    |   |   |    |      |
|      |      |              | you have in a    |   |   |    |      |
|      |      |              | tool is Floats,  |   |   |    |      |
|      |      |              | than that is     |   |   |    |      |
|      |      |              | what it will     |   |   |    |      |
|      |      |              | have to be)\     |   |   |    |      |
|      |      |              | - Map of         |   |   |    |      |
|      |      |              | committee cold   |   |   |    |      |
|      |      |              | key credentials  |   |   |    |      |
|      |      |              | that will be     |   |   |    |      |
|      |      |              | added to the     |   |   |    |      |
|      |      |              | committee with   |   |   |    |      |
|      |      |              | absolute epoch   |   |   |    |      |
|      |      |              | number number    |   |   |    |      |
|      |      |              | when they will   |   |   |    |      |
|      |      |              | expire           |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   |    |      |
|      |      |              | looking at an    |   |   |    |      |
|      |      |              | Update to the    |   |   |    |      |
|      |      |              | Constitution     |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I should be |   |   |    |      |
|      |      |              | able to see:\    |   |   |    |      |
|      |      |              | - The            |   |   |    |      |
|      |      |              | Constitution     |   |   |    |      |
|      |      |              | URL\             |   |   |    |      |
|      |      |              | - The            |   |   |    |      |
|      |      |              | Constitution     |   |   |    |      |
|      |      |              | hash\            |   |   |    |      |
|      |      |              | - The proposal   |   |   |    |      |
|      |      |              | policy script    |   |   |    |      |
|      |      |              | (if provided     |   |   |    |      |
|      |      |              | when the         |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action was       |   |   |    |      |
|      |      |              | submitted)       |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   |    |      |
|      |      |              | looking at a     |   |   |    |      |
|      |      |              | Hard Fork        |   |   |    |      |
|      |      |              | Initiation       |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I should be |   |   |    |      |
|      |      |              | able to see:\    |   |   |    |      |
|      |      |              | - The new major  |   |   |    |      |
|      |      |              | protocol version |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The          | Given that I am  |   |   | Vo | N    |
|      |      | governance   | reviewing the    |   |   | lt |      |
|      |      | action as    | details of a     |   |   | ai |      |
|      |      | displayed    | specific         |   |   | re |      |
|      |      | should       | governance       |   |   |    |      |
|      |      | include a    | action           |   |   |    |      |
|      |      | link to its  |                  |   |   |    |      |
|      |      | metadata     | When I click on  |   |   |    |      |
|      |      |              | the "view other  |   |   |    |      |
|      |      |              | details" link on |   |   |    |      |
|      |      |              | the governance   |   |   |    |      |
|      |      |              | action details   |   |   |    |      |
|      |      |              | page             |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Then I will be   |   |   |    |      |
|      |      |              | shown a warning  |   |   |    |      |
|      |      |              | asking if I want |   |   |    |      |
|      |      |              | to continue to   |   |   |    |      |
|      |      |              | an external url  |   |   |    |      |
|      |      |              | (which will be   |   |   |    |      |
|      |      |              | displayed). If I |   |   |    |      |
|      |      |              | continue then    |   |   |    |      |
|      |      |              | the external url |   |   |    |      |
|      |      |              | will open in a   |   |   |    |      |
|      |      |              | new tab.         |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Verify the   | Given that I am  |   |   | Vo | N    |
|      |      | integrity of | looking at a     |   |   | lt |      |
|      |      | a governance | governance       |   |   | ai |      |
|      |      | action's     | action           |   |   | re |      |
|      |      | metadata     |                  |   |   |    |      |
|      |      |              | Then I can see   |   |   |    |      |
|      |      |              | whether a hash   |   |   |    |      |
|      |      |              | of that          |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action's         |   |   |    |      |
|      |      |              | metadata matches |   |   |    |      |
|      |      |              | the *metadata    |   |   |    |      |
|      |      |              | hash* included   |   |   |    |      |
|      |      |              | in the anchor.   |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CH   | As a | Create a set | Given that I     |   |   | Vo | N    |
| .VO8 | p    | of keys      | have the CLI     |   |   | lt |      |
|      | oten |              | open in front of |   |   | ai |      |
|      | tial |              | me, when I run   |   |   | re |      |
|      | Co   |              | the              |   |   |    |      |
|      | nsti |              | corresponding    |   |   |    |      |
|      | tuti |              | command, then I  |   |   |    |      |
|      | onal |              | can verify that  |   |   |    |      |
|      | C    |              | I have created a |   |   |    |      |
|      | ommi |              | new key pair     |   |   |    |      |
|      | ttee |              |                  |   |   |    |      |
|      | Me   |              |                  |   |   |    |      |
|      | mber |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | want |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | come |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | Co   |              |                  |   |   |    |      |
|      | nsti |              |                  |   |   |    |      |
|      | tuti |              |                  |   |   |    |      |
|      | onal |              |                  |   |   |    |      |
|      | C    |              |                  |   |   |    |      |
|      | ommi |              |                  |   |   |    |      |
|      | ttee |              |                  |   |   |    |      |
|      | Me   |              |                  |   |   |    |      |
|      | mber |              |                  |   |   |    |      |
|      | so   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | vote |              |                  |   |   |    |      |
|      | on   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | orre |              |                  |   |   |    |      |
|      | spon |              |                  |   |   |    |      |
|      | ding |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | act  |              |                  |   |   |    |      |
|      | ions |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Include      | Given that I am  |   |   | Vo | N    |
|      |      | these keys   | using CLI and I  |   |   | lt |      |
|      |      | in a New     | have created my  |   |   | ai |      |
|      |      | Committee    | set of keys,     |   |   | re |      |
|      |      | Cold Key     | when they are    |   |   |    |      |
|      |      | Hash or      | registered in    |   |   |    |      |
|      |      | Script Hash  | the ledger, then |   |   |    |      |
|      |      |              | I can verify     |   |   |    |      |
|      |      |              | that my set of   |   |   |    |      |
|      |      |              | keys corresponds |   |   |    |      |
|      |      |              | to a CC member   |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Create an    | Given that I am  |   |   | CI | N    |
|      |      | a            | using CLI and I  |   |   | P- |      |
|      |      | uthorization | have created my  |   |   | 16 |      |
|      |      | certificate  | set of cold/hot  |   |   | 94 |      |
|      |      |              | key pairs, when  |   |   |    |      |
|      |      |              | I run the        |   |   | [[ |      |
|      |      |              | corresponding    |   |   | L9 |      |
|      |      |              | command, then I  |   |   | 93 |      |
|      |      |              | can verify that  |   |   | ]{ |      |
|      |      |              | the certificate  |   |   | .u |      |
|      |      |              | is stored        |   |   | nd |      |
|      |      |              | on-chain and it  |   |   | er |      |
|      |      |              | delegates rights |   |   | li |      |
|      |      |              | from the cold    |   |   | ne |      |
|      |      |              | key to the hot   |   |   | }] |      |
|      |      |              | key              |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | e7 |      |
|      |      |              |                  |   |   | 61 |      |
|      |      |              |                  |   |   | 20 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 05 |      |
|      |      |              |                  |   |   | 52 |      |
|      |      |              |                  |   |   | ef |      |
|      |      |              |                  |   |   | 62 |      |
|      |      |              |                  |   |   | 0d |      |
|      |      |              |                  |   |   | 96 |      |
|      |      |              |                  |   |   | 40 |      |
|      |      |              |                  |   |   | 1e |      |
|      |      |              |                  |   |   | d7 |      |
|      |      |              |                  |   |   | fd |      |
|      |      |              |                  |   |   | 3e |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | 1f |      |
|      |      |              |                  |   |   | 06 |      |
|      |      |              |                  |   |   | 2/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Only votes   | Given that my    |   |   | CI | N    |
|      |      | from active  | set of keys does |   |   | P- |      |
|      |      | Committee    | not correspond   |   |   | 16 |      |
|      |      | members are  | to an active CC  |   |   | 94 |      |
|      |      | considered.  | member, when I   |   |   |    |      |
|      |      |              | try to vote as a |   |   | [[ |      |
|      |      |              | CC member using  |   |   | L9 |      |
|      |      |              | CLI, then I get  |   |   | 93 |      |
|      |      |              | an error message |   |   | ]{ |      |
|      |      |              | telling me that  |   |   | .u |      |
|      |      |              | my credentials   |   |   | nd |      |
|      |      |              | are not valid    |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | e7 |      |
|      |      |              |                  |   |   | 61 |      |
|      |      |              |                  |   |   | 20 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 05 |      |
|      |      |              |                  |   |   | 52 |      |
|      |      |              |                  |   |   | ef |      |
|      |      |              |                  |   |   | 62 |      |
|      |      |              |                  |   |   | 0d |      |
|      |      |              |                  |   |   | 96 |      |
|      |      |              |                  |   |   | 40 |      |
|      |      |              |                  |   |   | 1e |      |
|      |      |              |                  |   |   | d7 |      |
|      |      |              |                  |   |   | fd |      |
|      |      |              |                  |   |   | 3e |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | 1f |      |
|      |      |              |                  |   |   | 06 |      |
|      |      |              |                  |   |   | 2/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
| CH   | As a | Access       | Given that I am  |   |   | Vo | N    |
| .VO9 | CC   | GovTool      | on the GovTool   |   |   | lt |      |
|      | Me   |              | homepage, when I |   |   | ai |      |
|      | mber |              | click the        |   |   | re |      |
|      | I    |              | "Governance      |   |   |    |      |
|      | want |              | actions" in the  |   |   |    |      |
|      | to   |              | topbar then I am |   |   |    |      |
|      | re   |              | sent to the      |   |   |    |      |
|      | view |              | governance       |   |   |    |      |
|      | a    |              | actions page.    |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | ac   |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | so   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | sc   |              |                  |   |   |    |      |
|      | ruti |              |                  |   |   |    |      |
|      | nise |              |                  |   |   |    |      |
|      | whe  |              |                  |   |   |    |      |
|      | ther |              |                  |   |   |    |      |
|      | or   |              |                  |   |   |    |      |
|      | not  |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | is   |              |                  |   |   |    |      |
|      | ali  |              |                  |   |   |    |      |
|      | gned |              |                  |   |   |    |      |
|      | with |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | Cons |              |                  |   |   |    |      |
|      | titu |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | See list of  | Given that I am  |   |   | Vo | N    |
|      |      | current      | on the           |   |   | lt |      |
|      |      | governance   | Governance       |   |   | ai |      |
|      |      | actions      | Actions page     |   |   | re |      |
|      |      |              | When I review    |   |   |    |      |
|      |      |              | the governance   |   |   |    |      |
|      |      |              | actions          |   |   |    |      |
|      |      |              | available to     |   |   |    |      |
|      |      |              | view on the      |   |   |    |      |
|      |      |              | page, then all   |   |   |    |      |
|      |      |              | of the non       |   |   |    |      |
|      |      |              | expired/         |   |   |    |      |
|      |      |              | ratified/enacted |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | actions.         |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | See details  | Given that I am  |   |   | Vo | N    |
|      |      | of a         | on the           |   |   | lt |      |
|      |      | specific     | Governance       |   |   | ai |      |
|      |      | governance   | Actions page,    |   |   | re |      |
|      |      | action       | When I click on  |   |   |    |      |
|      |      |              | an individual    |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action, Then I   |   |   |    |      |
|      |      |              | can see the      |   |   |    |      |
|      |      |              | relevant         |   |   |    |      |
|      |      |              | information      |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | See metadata | Given that I am  |   |   | Vo | N    |
|      |      |              | looking at an    |   |   | lt |      |
|      |      |              | individual       |   |   | ai |      |
|      |      |              | governance       |   |   | re |      |
|      |      |              | action page,     |   |   |    |      |
|      |      |              | when I click on  |   |   |    |      |
|      |      |              | "view other      |   |   |    |      |
|      |      |              | details" and I   |   |   |    |      |
|      |      |              | click on         |   |   |    |      |
|      |      |              | continue in the  |   |   |    |      |
|      |      |              | warning message, |   |   |    |      |
|      |      |              | Then an external |   |   |    |      |
|      |      |              | url will open in |   |   |    |      |
|      |      |              | a new tab.       |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Verify       | Given that I am  |   |   | Vo | N    |
|      |      | metadata     | looking at a     |   |   | lt |      |
|      |      | integrity    | governance       |   |   | ai |      |
|      |      |              | action then I    |   |   | re |      |
|      |      |              | can see whether  |   |   |    |      |
|      |      |              | a hash of that   |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action's         |   |   |    |      |
|      |      |              | metadata matches |   |   |    |      |
|      |      |              | the metadata     |   |   |    |      |
|      |      |              | hash included in |   |   |    |      |
|      |      |              | the anchor.      |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CH.  | As a | Find a       | Given that I am  |   |   | Vo | N    |
| VO10 | CC   | specific     | using CLI and I  |   |   | lt |      |
|      | Me   | governance   | know the         |   |   | ai |      |
|      | mber | action using | governance       |   |   | re |      |
|      | I    | CLI          | action ID, When  |   |   |    |      |
|      | want |              | I run the        |   |   |    |      |
|      | to   |              | command to       |   |   |    |      |
|      | vote |              | review a         |   |   |    |      |
|      | on a |              | specific         |   |   |    |      |
|      | go   |              | governance       |   |   |    |      |
|      | vern |              | action, Then I   |   |   |    |      |
|      | ance |              | can see the      |   |   |    |      |
|      | ac   |              | details of that  |   |   |    |      |
|      | tion |              | individual       |   |   |    |      |
|      | so   |              | governance       |   |   |    |      |
|      | that |              | action.          |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | app  |              |                  |   |   |    |      |
|      | rove |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | act  |              |                  |   |   |    |      |
|      | ions |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | lign |              |                  |   |   |    |      |
|      | with |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | cons |              |                  |   |   |    |      |
|      | titu |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Vote as a    | Given that I am  |   |   | Vo | N    |
|      |      | Co           | using CLI and I  |   |   | lt |      |
|      |      | nstitutional | know the         |   |   | ai |      |
|      |      | Committee    | governance       |   |   | re |      |
|      |      | member using | action ID, When  |   |   |    |      |
|      |      | CLI          | I build the      |   |   |    |      |
|      |      |              | transaction to   |   |   |    |      |
|      |      |              | vote on a        |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action, Then I   |   |   |    |      |
|      |      |              | can specify my   |   |   |    |      |
|      |      |              | role (ccm), the  |   |   |    |      |
|      |      |              | action ID, and   |   |   |    |      |
|      |      |              | the intent to    |   |   |    |      |
|      |      |              | vote             |   |   |    |      |
|      |      |              | (YES/NO/ABSTAIN) |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      |              | Given that I am  |   |   | Vo | N    |
|      |      |              | using CLI and I  |   |   | lt |      |
|      |      |              | have built the   |   |   | ai |      |
|      |      |              | transaction to   |   |   | re |      |
|      |      |              | vote on a        |   |   |    |      |
|      |      |              | specific         |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action, When I   |   |   |    |      |
|      |      |              | run the command  |   |   |    |      |
|      |      |              | to sign the      |   |   |    |      |
|      |      |              | transaction,     |   |   |    |      |
|      |      |              | Then I can       |   |   |    |      |
|      |      |              | submit the       |   |   |    |      |
|      |      |              | transaction and  |   |   |    |      |
|      |      |              | pay the          |   |   |    |      |
|      |      |              | transaction      |   |   |    |      |
|      |      |              | costs            |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Provide      | Given that I am  |   |   | Vo | N    |
|      |      | rationale    | using CLI, When  |   |   | lt |      |
|      |      | for vote     | I am building a  |   |   | ai |      |
|      |      | with a       | transaction to   |   |   | re |      |
|      |      | metadata     | vote on a        |   |   |    |      |
|      |      | anchor       | specific         |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action, Then I   |   |   |    |      |
|      |      |              | can use the      |   |   |    |      |
|      |      |              | metadata anchor  |   |   |    |      |
|      |      |              | to provide a     |   |   |    |      |
|      |      |              | rationale for my |   |   |    |      |
|      |      |              | vote             |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Change vote  | Given that I     |   |   | Vo | N    |
|      |      |              | have submitted a |   |   | lt |      |
|      |      |              | vote on a        |   |   | ai |      |
|      |      |              | specific         |   |   | re |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action, When I   |   |   |    |      |
|      |      |              | vote again on    |   |   |    |      |
|      |      |              | the same         |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | action, Then I   |   |   |    |      |
|      |      |              | can change the   |   |   |    |      |
|      |      |              | intent to vote   |   |   |    |      |
|      |      |              | (YES/NO/ABSTAIN) |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CH.  | As a | Create a new | Given that I am  |   |   | Vo | N    |
| VO11 | CC   | a            | a CC member and  |   |   | lt |      |
|      | Me   | uthorization | I have enough    |   |   | ai |      |
|      | mber | certificate  | funds to pay the |   |   | re |      |
|      | I    |              | transaction      |   |   |    |      |
|      | want |              | fees, When I     |   |   |    |      |
|      | to   |              | create a new     |   |   |    |      |
|      | ch   |              | authorisation    |   |   |    |      |
|      | ange |              | certificate      |   |   |    |      |
|      | my   |              | using the same   |   |   |    |      |
|      | vo   |              | cold key, Then a |   |   |    |      |
|      | ting |              | new hot key is   |   |   |    |      |
|      | cre  |              | authorised to    |   |   |    |      |
|      | dent |              | vote as a valid  |   |   |    |      |
|      | ials |              | CC member        |   |   |    |      |
|      | so I |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | ma   |              |                  |   |   |    |      |
|      | nage |              |                  |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | or   |              |                  |   |   |    |      |
|      | gani |              |                  |   |   |    |      |
|      | sati |              |                  |   |   |    |      |
|      | on's |              |                  |   |   |    |      |
|      | vo   |              |                  |   |   |    |      |
|      | ting |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CH.  | As a | Create a     | Given that I am  |   |   | Vo | N    |
| VO12 | CC   | resignation  | a CC member and  |   |   | lt |      |
|      | Me   | certificate  | I have enough    |   |   | ai |      |
|      | mber |              | funds to pay the |   |   | re |      |
|      | I    |              | transaction      |   |   |    |      |
|      | want |              | fees, When I     |   |   |    |      |
|      | to   |              | create a         |   |   |    |      |
|      | re   |              | resignation      |   |   |    |      |
|      | tire |              | certificate,     |   |   |    |      |
|      | so   |              | Then my cold key |   |   |    |      |
|      | my   |              | and the derived  |   |   |    |      |
|      | cre  |              | hote keys are no |   |   |    |      |
|      | dent |              | longer valid to  |   |   |    |      |
|      | ials |              | vote as a CC     |   |   |    |      |
|      | are  |              | member           |   |   |    |      |
|      | no   |              |                  |   |   |    |      |
|      | lo   |              |                  |   |   |    |      |
|      | nger |              |                  |   |   |    |      |
|      | v    |              |                  |   |   |    |      |
|      | alid |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CH.  | As a | *Correct     | Detail pending   |   | D | A  |      |
| CLI1 | Pl   | operation of |                  |   | e | PI |      |
|      | utus | BLS          |                  |   | t | /C |      |
|      | d    | primitives.* |                  |   | a | LI |      |
|      | evel |              |                  |   | i |    |      |
|      | oper | *Correct     |                  |   | l |    |      |
|      | I    | operation of |                  |   | p |    |      |
|      | want | new bitwise  |                  |   | e |    |      |
|      | the  | primitives.* |                  |   | n |    |      |
|      | Node |              |                  |   | d |    |      |
|      | to   | *New Plutus  |                  |   | i |    |      |
|      | sup  | V3 cost      |                  |   | n |    |      |
|      | port | model is     |                  |   | g |    |      |
|      | Pl   | used         |                  |   |   |    |      |
|      | utus | correctly    |                  |   |   |    |      |
|      | V3   | for the new  |                  |   |   |    |      |
|      | requ | primitives.* |                  |   |   |    |      |
|      | irem |              |                  |   |   |    |      |
|      | ents | *Plutus      |                  |   |   |    |      |
|      | for  | scripts are  |                  |   |   |    |      |
|      | CIP- | correctly    |                  |   |   |    |      |
|      | 1694 | used for     |                  |   |   |    |      |
|      |      | DRep         |                  |   |   |    |      |
|      |      | voting.*     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | *Plutus      |                  |   |   |    |      |
|      |      | scripts on   |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | constitution |                  |   |   |    |      |
|      |      | correctly    |                  |   |   |    |      |
|      |      | control CC   |                  |   |   |    |      |
|      |      | voting.*     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | *Benchmark   |                  |   |   |    |      |
|      |      | execution    |                  |   |   |    |      |
|      |      | times are    |                  |   |   |    |      |
|      |      | within       |                  |   |   |    |      |
|      |      | acceptable   |                  |   |   |    |      |
|      |      | range.*      |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CH.A | Le   | This is a    | Detail pending   |   |   | A  | U    |
| PI11 | dger | placeholder  |                  |   |   | PI | PDAT |
|      | API  |              |                  |   |   | /C | E/RE |
|      | User |              |                  |   |   | LI | MOVE |
|      | S    |              |                  |   |   |    |      |
|      | tory |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| VO16 | SPO  |              |                  |   |   | A  | U    |
|      | I    |              |                  |   |   | PI | PDAT |
|      | nter |              |                  |   |   | /C | E/RE |
|      | face |              |                  |   |   | LI | MOVE |
|      | User |              |                  |   |   |    |      |
|      | S    |              |                  |   |   |    |      |
|      | tory |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| INT1 | As a |              | Detail pending   |   |   |    |      |
|      | user |              |                  |   |   |    |      |
|      | of   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | sy   |              |                  |   |   |    |      |
|      | stem |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | want |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | act  |              |                  |   |   |    |      |
|      | ions |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | orre |              |                  |   |   |    |      |
|      | ctly |              |                  |   |   |    |      |
|      | s    |              |                  |   |   |    |      |
|      | ubmi |              |                  |   |   |    |      |
|      | tted |              |                  |   |   |    |      |
|      | on   |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| *I   | *As  | *(voter      | Detail pending   |   |   |    |      |
| NT2* | a    | type,        |                  |   |   |    |      |
|      | user | thresholds,  |                  |   |   |    |      |
|      | of   | DRep         |                  |   |   |    |      |
|      | the  | activity)*   |                  |   |   |    |      |
|      | sy   |              |                  |   |   |    |      |
|      | stem |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | want |              |                  |   |   |    |      |
|      | All  |              |                  |   |   |    |      |
|      | act  |              |                  |   |   |    |      |
|      | ions |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | rati |              |                  |   |   |    |      |
|      | fied |              |                  |   |   |    |      |
|      | on-c |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | orre |              |                  |   |   |    |      |
|      | ctly |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | ccor |              |                  |   |   |    |      |
|      | ding |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | CIP- |              |                  |   |   |    |      |
|      | 1694 |              |                  |   |   |    |      |
|      | ru   |              |                  |   |   |    |      |
|      | les* |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| *I   | *As  | Timely       |                  |   |   |    |      |
| NT3* | a    |              |                  |   |   |    |      |
|      | user |              |                  |   |   |    |      |
|      | of   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | sy   |              |                  |   |   |    |      |
|      | stem |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | want |              |                  |   |   |    |      |
|      | All  |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | act  |              |                  |   |   |    |      |
|      | ions |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | ena  |              |                  |   |   |    |      |
|      | cted |              |                  |   |   |    |      |
|      | on   |              |                  |   |   |    |      |
|      | time |              |                  |   |   |    |      |
|      | on-c |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
|      | f    |              |                  |   |   |    |      |
|      | ollo |              |                  |   |   |    |      |
|      | wing |              |                  |   |   |    |      |
|      | r    |              |                  |   |   |    |      |
|      | atif |              |                  |   |   |    |      |
|      | icat |              |                  |   |   |    |      |
|      | ion* |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Correctly    |                  |   |   |    |      |
|      |      | according to |                  |   |   |    |      |
|      |      | CIP-1694     |                  |   |   |    |      |
|      |      | rule         |                  |   |   |    |      |
|      |      | s:*Parameter |                  |   |   |    |      |
|      |      | updates,     |                  |   |   |    |      |
|      |      | Info, Hard   |                  |   |   |    |      |
|      |      | Forks, No    |                  |   |   |    |      |
|      |      | Confidence,  |                  |   |   |    |      |
|      |      | New          |                  |   |   |    |      |
|      |      | Committee,   |                  |   |   |    |      |
|      |      | New          |                  |   |   |    |      |
|      |      | C            |                  |   |   |    |      |
|      |      | onstitution, |                  |   |   |    |      |
|      |      | Treasury     |                  |   |   |    |      |
|      |      | Withdrawals. |                  |   |   |    |      |
|      |      | This will    |                  |   |   |    |      |
|      |      | expand into  |                  |   |   |    |      |
|      |      | many         |                  |   |   |    |      |
|      |      | re           |                  |   |   |    |      |
|      |      | quirements.* |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| SY   |      |              |                  |   |   |    |      |
| STEM |      |              |                  |   |   |    |      |
| L    |      |              |                  |   |   |    |      |
| EVEL |      |              |                  |   |   |    |      |
| (not |      |              |                  |   |   |    |      |
| f    |      |              |                  |   |   |    |      |
| ully |      |              |                  |   |   |    |      |
| c    |      |              |                  |   |   |    |      |
| ompl |      |              |                  |   |   |    |      |
| eted |      |              |                  |   |   |    |      |
| yet) |      |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| [[C  | As   | Hash value   | Given that I     |   | D | CI |      |
| IP1] | any  | of the       | access a Cardano |   | e | P- |      |
| {.un | per  | off-chain    | Explorer and     |   | t | 16 |      |
| derl | sona | Constitution | that it display  |   | a | 94 |      |
| ine} |      | is recorded  | the ledger       |   | i |    |      |
| ](ht | I    | on-chain     | states           |   | l | [[ |      |
| tps: | want |              | accurately, Then |   | P | L9 |      |
| //do | the  |              | I can access a   |   | e | 58 |      |
| cs.g | hash |              | map of the       |   | n | ]{ |      |
| oogl | v    |              | current          |   | d | .u |      |
| e.co | alue |              | constitution     |   | i | nd |      |
| m/do | of   |              | hash and the URL |   | n | er |      |
| cume | the  |              | of the off-chain |   | g | li |      |
| nt/d | o    |              | document         |   |   | ne |      |
| /1Ym | ff-c |              |                  |   |   | }] |      |
| j_Fo | hain |              |                  |   |   | (h |      |
| h3lV | Cons |              |                  |   |   | tt |      |
| Yq2a | titu |              |                  |   |   | ps |      |
| sI5W | tion |              |                  |   |   | :/ |      |
| EdQY | to   |              |                  |   |   | /g |      |
| Bud5 | be   |              |                  |   |   | it |      |
| B8Kb | reco |              |                  |   |   | hu |      |
| Jcw4 | rded |              |                  |   |   | b. |      |
| jpUw | on-c |              |                  |   |   | co |      |
| uv5p | hain |              |                  |   |   | m/ |      |
| 8/ed |      |              |                  |   |   | ca |      |
| it#b | So   |              |                  |   |   | rd |      |
| ookm | that |              |                  |   |   | an |      |
| ark= | I    |              |                  |   |   | o- |      |
| id.y | can  |              |                  |   |   | fo |      |
| zo1a | ve   |              |                  |   |   | un |      |
| ziuw | rify |              |                  |   |   | da |      |
| sxs) | the  |              |                  |   |   | ti |      |
|      | auth |              |                  |   |   | on |      |
|      | enti |              |                  |   |   | /C |      |
|      | city |              |                  |   |   | IP |      |
|      | of   |              |                  |   |   | s/ |      |
|      | the  |              |                  |   |   | bl |      |
|      | o    |              |                  |   |   | ob |      |
|      | ff-c |              |                  |   |   | /d |      |
|      | hain |              |                  |   |   | e7 |      |
|      | docu |              |                  |   |   | 61 |      |
|      | ment |              |                  |   |   | 20 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 05 |      |
|      |      |              |                  |   |   | 52 |      |
|      |      |              |                  |   |   | ef |      |
|      |      |              |                  |   |   | 62 |      |
|      |      |              |                  |   |   | 0d |      |
|      |      |              |                  |   |   | 96 |      |
|      |      |              |                  |   |   | 40 |      |
|      |      |              |                  |   |   | 1e |      |
|      |      |              |                  |   |   | d7 |      |
|      |      |              |                  |   |   | fd |      |
|      |      |              |                  |   |   | 3e |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | 1f |      |
|      |      |              |                  |   |   | 06 |      |
|      |      |              |                  |   |   | 2/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 95 |      |
|      |      |              |                  |   |   | 8C |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | -L |      |
|      |      |              |                  |   |   | 95 |      |
|      |      |              |                  |   |   | 8C |      |
|      |      |              |                  |   |   | 12 |      |
|      |      |              |                  |   |   | 0) |      |
+------+------+--------------+------------------+---+---+----+------+
| [[C  | As   | Committee    | Given that the   |   | D | CI |      |
| IP2] | an   | members key  | node is up to    |   | e | P- |      |
| {.un | ada  | hashes must  | date, then it    |   | t | 16 |      |
| derl | ho   | be recorded  | should include a |   | a | 94 |      |
| ine} | lder | on chain and | record for each  |   | i |    |      |
| ](ht |      | be publicly  | committee member |   | l | [[ |      |
| tps: | I    | accessible   | detailing their  |   | P | L9 |      |
| //do | want |              | key-hashes, term |   | e | 93 |      |
| cs.g | the  | ADA holder   | information (end |   | n | ]{ |      |
| oogl | key  | must be able | epochs), and the |   | d | .u |      |
| e.co | hash | to check     | corresponding    |   | i | nd |      |
| m/do | of   | that the key | cold to hot key  |   | n | er |      |
| cume | ac   | hashes of    | authorization    |   | g | li |      |
| nt/d | tive | active and   | maps.            |   |   | ne |      |
| /1Ym | and  | expired      |                  |   |   | }] |      |
| j_Fo | exp  | committee    |                  |   |   | (h |      |
| h3lV | ired | members are  |                  |   |   | tt |      |
| Yq2a | C    | registered   |                  |   |   | ps |      |
| sI5W | ommi | on-chain     |                  |   |   | :/ |      |
| EdQY | ttee | status       |                  |   |   | /g |      |
| Bud5 | Mem  |              |                  |   |   | it |      |
| B8Kb | bers |              |                  |   |   | hu |      |
| Jcw4 | and  |              |                  |   |   | b. |      |
| jpUw | t    |              |                  |   |   | co |      |
| uv5p | heir |              |                  |   |   | m/ |      |
| 8/ed | t    |              |                  |   |   | ca |      |
| it#b | erms |              |                  |   |   | rd |      |
| ookm | to   |              |                  |   |   | an |      |
| ark= | be   |              |                  |   |   | o- |      |
| id.e | re   |              |                  |   |   | fo |      |
| lqu6 | gist |              |                  |   |   | un |      |
| qa8l | ered |              |                  |   |   | da |      |
| tse) | on-c |              |                  |   |   | ti |      |
|      | hain |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      | So   |              |                  |   |   | IP |      |
|      | that |              |                  |   |   | s/ |      |
|      | the  |              |                  |   |   | bl |      |
|      | sy   |              |                  |   |   | ob |      |
|      | stem |              |                  |   |   | /d |      |
|      | can  |              |                  |   |   | e7 |      |
|      | c    |              |                  |   |   | 61 |      |
|      | ount |              |                  |   |   | 20 |      |
|      | t    |              |                  |   |   | a3 |      |
|      | heir |              |                  |   |   | 05 |      |
|      | v    |              |                  |   |   | 52 |      |
|      | otes |              |                  |   |   | ef |      |
|      |      |              |                  |   |   | 62 |      |
|      |      |              |                  |   |   | 0d |      |
|      |      |              |                  |   |   | 96 |      |
|      |      |              |                  |   |   | 40 |      |
|      |      |              |                  |   |   | 1e |      |
|      |      |              |                  |   |   | d7 |      |
|      |      |              |                  |   |   | fd |      |
|      |      |              |                  |   |   | 3e |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | 1f |      |
|      |      |              |                  |   |   | 06 |      |
|      |      |              |                  |   |   | 2/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
| [[C  | As   | It must be   | Any ada holder   |   | D | CI |      |
| IP3] | an   | possible to  | can submit a     |   | e | P- |      |
| {.un | ada  | replace the  | governance       |   | t | 16 |      |
| derl | ho   | co           | action that      |   | a | 94 |      |
| ine} | lder | nstitutional | proposes to add  |   | i |    |      |
| ](ht |      | committee    | or remove one or |   | l | [[ |      |
| tps: | I    | via a        | many new         |   | P | L9 |      |
| //do | want | governance   | committee        |   | e | 97 |      |
| cs.g | to   | action       | members.         |   | n | ]{ |      |
| oogl | be   |              |                  |   | d | .u |      |
| e.co | able |              | Given that a     |   | i | nd |      |
| m/do | to   |              | governance       |   | n | er |      |
| cume | su   |              | action to update |   | g | li |      |
| nt/d | bmit |              | the committee    |   |   | ne |      |
| /1Ym | a    |              | has been         |   |   | }] |      |
| j_Fo | prop |              | proposed And     |   |   | (h |      |
| h3lV | osal |              | both SPO and     |   |   | tt |      |
| Yq2a | to   |              | DRep YES votes   |   |   | ps |      |
| sI5W | rep  |              | are equal or     |   |   | :/ |      |
| EdQY | lace |              | greater than the |   |   | /g |      |
| Bud5 | all  |              | required         |   |   | it |      |
| B8Kb | or   |              | threshold        |   |   | hu |      |
| Jcw4 | part |              | (depending on    |   |   | b. |      |
| jpUw | of   |              | state of         |   |   | co |      |
| uv5p | the  |              | no-confidence or |   |   | m/ |      |
| 8/ed | cur  |              | normal state)    |   |   | ca |      |
| it#b | rent |              |                  |   |   | rd |      |
| ookm | co   |              | The governance   |   |   | an |      |
| ark= | nsti |              | action is        |   |   | o- |      |
| id.p | tuti |              | ratified and     |   |   | fo |      |
| ddqk | onal |              | enacted          |   |   | un |      |
| syfs | c    |              | automatically at |   |   | da |      |
| hgc) | ommi |              | the next epoch   |   |   | ti |      |
|      | ttee |              | transition,      |   |   | on |      |
|      |      |              | otherwise it's   |   |   | /C |      |
|      | So   |              | expired.         |   |   | IP |      |
|      | that |              |                  |   |   | s/ |      |
|      | c    |              |                  |   |   | bl |      |
|      | ommi |              |                  |   |   | ob |      |
|      | ttee |              |                  |   |   | /d |      |
|      | mem  |              |                  |   |   | e7 |      |
|      | bers |              |                  |   |   | 61 |      |
|      | that |              |                  |   |   | 20 |      |
|      | have |              |                  |   |   | a3 |      |
|      | lost |              |                  |   |   | 05 |      |
|      | co   |              |                  |   |   | 52 |      |
|      | nfid |              |                  |   |   | ef |      |
|      | ence |              |                  |   |   | 62 |      |
|      | of   |              |                  |   |   | 0d |      |
|      | ada  |              |                  |   |   | 96 |      |
|      | hol  |              |                  |   |   | 40 |      |
|      | ders |              |                  |   |   | 1e |      |
|      | can  |              |                  |   |   | d7 |      |
|      | be   |              |                  |   |   | fd |      |
|      | rem  |              |                  |   |   | 3e |      |
|      | oved |              |                  |   |   | 5b |      |
|      | from |              |                  |   |   | ca |      |
|      | t    |              |                  |   |   | 1f |      |
|      | heir |              |                  |   |   | 06 |      |
|      | dut  |              |                  |   |   | 2/ |      |
|      | ies. |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 7C |      |
|      |      |              |                  |   |   | 1- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 97 |      |
|      |      |              |                  |   |   | C7 |      |
|      |      |              |                  |   |   | 8) |      |
+------+------+--------------+------------------+---+---+----+------+
| [[C  | As   | Size of the  | Detail Pending   |   | D | [[ |      |
| IP4] | an   | co           |                  |   | e | L1 |      |
| {.un | ada  | nstitutional |                  |   | t | 00 |      |
| derl | ho   | committee    |                  |   | a | 9] |      |
| ine} | lder | must be      |                  |   | i | {. |      |
| ](ht |      | variable     |                  |   | l | un |      |
| tps: | I    |              |                  |   | P | de |      |
| //do | want |              |                  |   | e | rl |      |
| cs.g | the  |              |                  |   | n | in |      |
| oogl | size |              |                  |   | d | e} |      |
| e.co | of   |              |                  |   | i | ]( |      |
| m/do | the  |              |                  |   | n | ht |      |
| cume | co   |              |                  |   | g | tp |      |
| nt/d | nsti |              |                  |   |   | s: |      |
| /1Ym | tuti |              |                  |   |   | // |      |
| j_Fo | onal |              |                  |   |   | gi |      |
| h3lV | c    |              |                  |   |   | th |      |
| Yq2a | ommi |              |                  |   |   | ub |      |
| sI5W | ttee |              |                  |   |   | .c |      |
| EdQY |      |              |                  |   |   | om |      |
| Bud5 | To   |              |                  |   |   | /c |      |
| B8Kb | be   |              |                  |   |   | ar |      |
| Jcw4 | n    |              |                  |   |   | da |      |
| jpUw | ot-f |              |                  |   |   | no |      |
| uv5p | ixed |              |                  |   |   | -f |      |
| 8/ed |      |              |                  |   |   | ou |      |
| it#b | So   |              |                  |   |   | nd |      |
| ookm | that |              |                  |   |   | at |      |
| ark= | I    |              |                  |   |   | io |      |
| id.m | can  |              |                  |   |   | n/ |      |
| ca6c | pro  |              |                  |   |   | CI |      |
| vcoh | pose |              |                  |   |   | Ps |      |
| t53) | a    |              |                  |   |   | /b |      |
|      | d    |              |                  |   |   | lo |      |
|      | iffe |              |                  |   |   | b/ |      |
|      | rent |              |                  |   |   | ad |      |
|      | size |              |                  |   |   | a2 |      |
|      | via  |              |                  |   |   | cf |      |
|      | a    |              |                  |   |   | 6a |      |
|      | go   |              |                  |   |   | 9e |      |
|      | vern |              |                  |   |   | 27 |      |
|      | ance |              |                  |   |   | fb |      |
|      | ac   |              |                  |   |   | df |      |
|      | tion |              |                  |   |   | 37 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | 1b |      |
|      |      |              |                  |   |   | e0 |      |
|      |      |              |                  |   |   | 78 |      |
|      |      |              |                  |   |   | 03 |      |
|      |      |              |                  |   |   | 71 |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | ab |      |
|      |      |              |                  |   |   | 2b |      |
|      |      |              |                  |   |   | 77 |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L1 |      |
|      |      |              |                  |   |   | 00 |      |
|      |      |              |                  |   |   | 9) |      |
+------+------+--------------+------------------+---+---+----+------+
| [[C  | As   | Size of      | Detail Pending   |   | D | [[ |      |
| IP5] | an   | committee    |                  |   | e | L1 |      |
| {.un | ada  | threshold    |                  |   | t | 01 |      |
| derl | hol  | must be      |                  |   | a | 1] |      |
| ine} | der, | variable     |                  |   | i | {. |      |
| ](ht |      |              |                  |   | l | un |      |
| tps: | I    |              |                  |   | P | de |      |
| //do | want |              |                  |   | e | rl |      |
| cs.g | that |              |                  |   | n | in |      |
| oogl | the  |              |                  |   | d | e} |      |
| e.co | c    |              |                  |   | i | ]( |      |
| m/do | ommi |              |                  |   | n | ht |      |
| cume | ttee |              |                  |   | g | tp |      |
| nt/d | t    |              |                  |   |   | s: |      |
| /1Ym | hres |              |                  |   |   | // |      |
| j_Fo | hold |              |                  |   |   | gi |      |
| h3lV | (the |              |                  |   |   | th |      |
| Yq2a | frac |              |                  |   |   | ub |      |
| sI5W | tion |              |                  |   |   | .c |      |
| EdQY | of   |              |                  |   |   | om |      |
| Bud5 | c    |              |                  |   |   | /c |      |
| B8Kb | ommi |              |                  |   |   | ar |      |
| Jcw4 | ttee |              |                  |   |   | da |      |
| jpUw | is   |              |                  |   |   | no |      |
| uv5p | not  |              |                  |   |   | -f |      |
| 8/ed | f    |              |                  |   |   | ou |      |
| it#b | ixed |              |                  |   |   | nd |      |
| ookm |      |              |                  |   |   | at |      |
| ark= | So   |              |                  |   |   | io |      |
| id.t | that |              |                  |   |   | n/ |      |
| dyxk | I    |              |                  |   |   | CI |      |
| 950f | can  |              |                  |   |   | Ps |      |
| 5v8) | pro  |              |                  |   |   | /b |      |
|      | pose |              |                  |   |   | lo |      |
|      | a    |              |                  |   |   | b/ |      |
|      | d    |              |                  |   |   | ad |      |
|      | iffe |              |                  |   |   | a2 |      |
|      | rent |              |                  |   |   | cf |      |
|      | t    |              |                  |   |   | 6a |      |
|      | hres |              |                  |   |   | 9e |      |
|      | hold |              |                  |   |   | 27 |      |
|      | via  |              |                  |   |   | fb |      |
|      | a    |              |                  |   |   | df |      |
|      | go   |              |                  |   |   | 37 |      |
|      | vern |              |                  |   |   | ca |      |
|      | ance |              |                  |   |   | 1b |      |
|      | ac   |              |                  |   |   | e0 |      |
|      | tion |              |                  |   |   | 78 |      |
|      |      |              |                  |   |   | 03 |      |
|      |      |              |                  |   |   | 71 |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | ab |      |
|      |      |              |                  |   |   | 2b |      |
|      |      |              |                  |   |   | 77 |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L1 |      |
|      |      |              |                  |   |   | 01 |      |
|      |      |              |                  |   |   | 1) |      |
+------+------+--------------+------------------+---+---+----+------+
| CIP6 | As   | Users must   | Detail Pending   |   | D | [[ |      |
|      | an   | be able to   |                  |   | e | L1 |      |
|      | ada  | elect an     |                  |   | t | 01 |      |
|      | ho   | empty        |                  |   | a | 4] |      |
|      | lder | committee    |                  |   | i | {. |      |
|      |      |              |                  |   | l | un |      |
|      | I    | Ratifying    |                  |   | P | de |      |
|      | want | governance   |                  |   | e | rl |      |
|      | to   | actions must |                  |   | n | in |      |
|      | be   | be possible  |                  |   | d | e} |      |
|      | able | without      |                  |   | i | ]( |      |
|      | to   | co           |                  |   | n | ht |      |
|      | have | nstitutional |                  |   | g | tp |      |
|      | e    | committee    |                  |   |   | s: |      |
|      | lect |              |                  |   |   | // |      |
|      | an   |              |                  |   |   | gi |      |
|      | e    |              |                  |   |   | th |      |
|      | mpty |              |                  |   |   | ub |      |
|      | c    |              |                  |   |   | .c |      |
|      | ommi |              |                  |   |   | om |      |
|      | ttee |              |                  |   |   | /c |      |
|      | if   |              |                  |   |   | ar |      |
|      | the  |              |                  |   |   | da |      |
|      | c    |              |                  |   |   | no |      |
|      | ommu |              |                  |   |   | -f |      |
|      | nity |              |                  |   |   | ou |      |
|      | wi   |              |                  |   |   | nd |      |
|      | shes |              |                  |   |   | at |      |
|      | to   |              |                  |   |   | io |      |
|      | abo  |              |                  |   |   | n/ |      |
|      | lish |              |                  |   |   | CI |      |
|      | the  |              |                  |   |   | Ps |      |
|      | co   |              |                  |   |   | /b |      |
|      | nsti |              |                  |   |   | lo |      |
|      | tuti |              |                  |   |   | b/ |      |
|      | onal |              |                  |   |   | ad |      |
|      | c    |              |                  |   |   | a2 |      |
|      | ommi |              |                  |   |   | cf |      |
|      | ttee |              |                  |   |   | 6a |      |
|      | enti |              |                  |   |   | 9e |      |
|      | rely |              |                  |   |   | 27 |      |
|      |      |              |                  |   |   | fb |      |
|      | So   |              |                  |   |   | df |      |
|      | that |              |                  |   |   | 37 |      |
|      | SPO  |              |                  |   |   | ca |      |
|      | and  |              |                  |   |   | 1b |      |
|      | D    |              |                  |   |   | e0 |      |
|      | reps |              |                  |   |   | 78 |      |
|      | can  |              |                  |   |   | 03 |      |
|      | cont |              |                  |   |   | 71 |      |
|      | inue |              |                  |   |   | fb |      |
|      | to   |              |                  |   |   | ab |      |
|      | ra   |              |                  |   |   | 2b |      |
|      | tify |              |                  |   |   | 77 |      |
|      | go   |              |                  |   |   | 48 |      |
|      | vern |              |                  |   |   | /C |      |
|      | ance |              |                  |   |   | IP |      |
|      | act  |              |                  |   |   | -1 |      |
|      | ions |              |                  |   |   | 69 |      |
|      | wit  |              |                  |   |   | 4/ |      |
|      | hout |              |                  |   |   | RE |      |
|      | the  |              |                  |   |   | AD |      |
|      | need |              |                  |   |   | ME |      |
|      | of a |              |                  |   |   | .m |      |
|      | co   |              |                  |   |   | d? |      |
|      | nsti |              |                  |   |   | pl |      |
|      | tuti |              |                  |   |   | ai |      |
|      | onal |              |                  |   |   | n= |      |
|      | c    |              |                  |   |   | 1# |      |
|      | ommi |              |                  |   |   | L1 |      |
|      | ttee |              |                  |   |   | 01 |      |
|      |      |              |                  |   |   | 4) |      |
+------+------+--------------+------------------+---+---+----+------+
| CIP7 | As   | There must   | Detail Pending   |   | D | CI |      |
|      | an   | be a command |                  |   | e | P- |      |
|      | Ada  | in in the    |                  |   | t | 16 |      |
|      | hol  | Cardano CLI  |                  |   | a | 94 |      |
|      | der, | allowing the |                  |   | i |    |      |
|      |      | user to      |                  |   | l |    |      |
|      | I    | submit a     |                  |   | P |    |      |
|      | want | governance   |                  |   | e |    |      |
|      | to   | action       |                  |   | n |    |      |
|      | su   |              |                  |   | d |    |      |
|      | bmit | The input    |                  |   | i |    |      |
|      | a    | must include |                  |   | n |    |      |
|      | go   | validation   |                  |   | g |    |      |
|      | vern | checks for   |                  |   |   |    |      |
|      | ance | format and   |                  |   |   |    |      |
|      | act  | criteria     |                  |   |   |    |      |
|      | ion, |              |                  |   |   |    |      |
|      |      | After        |                  |   |   |    |      |
|      | So   | successful   |                  |   |   |    |      |
|      | that | validation   |                  |   |   |    |      |
|      | it   | the          |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | be   | user must be |                  |   |   |    |      |
|      | co   | informed of  |                  |   |   |    |      |
|      | nsid | confirmation |                  |   |   |    |      |
|      | ered | through the  |                  |   |   |    |      |
|      | by   | CLI          |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | go   | An action    |                  |   |   |    |      |
|      | vern | should have  |                  |   |   |    |      |
|      | ance | an accepted  |                  |   |   |    |      |
|      | bod  | or rejected  |                  |   |   |    |      |
|      | ies/ | status?      |                  |   |   |    |      |
|      | proc |              |                  |   |   |    |      |
|      | ess. |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CIP8 | As a | DReps must   | Given that a     |   | D | CI |      |
|      | dele | have access  | Drep has casted  |   | e | P- |      |
|      | gate | to the list  | a vote the       |   | t | 16 |      |
|      | re   | of current   | system           |   | a | 94 |      |
|      | pres | governance   | accurately       |   | i |    |      |
|      | enta | actions (can | records and      |   | l |    |      |
|      | tive | we specify   | reflects these   |   | P |    |      |
|      | (DR  | where they   | votes.           |   | e |    |      |
|      | ep), | get it?).    |                  |   | n |    |      |
|      |      |              |                  |   | d |    |      |
|      | I    | DReps should |                  |   | i |    |      |
|      | want | be able to   |                  |   | n |    |      |
|      | to   | cast their   |                  |   | g |    |      |
|      | vote | vote on each |                  |   |   |    |      |
|      | on   | action       |                  |   |   |    |      |
|      | s    | (through the |                  |   |   |    |      |
|      | ubmi | CL or        |                  |   |   |    |      |
|      | tted | through an   |                  |   |   |    |      |
|      | go   | app)?        |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance | An action    |                  |   |   |    |      |
|      | acti | should have  |                  |   |   |    |      |
|      | ons, | an accepted  |                  |   |   |    |      |
|      |      | or rejected  |                  |   |   |    |      |
|      | So   | status?      |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | r    |              |                  |   |   |    |      |
|      | epre |              |                  |   |   |    |      |
|      | sent |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | i    |              |                  |   |   |    |      |
|      | nter |              |                  |   |   |    |      |
|      | ests |              |                  |   |   |    |      |
|      | of   |              |                  |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | de   |              |                  |   |   |    |      |
|      | lega |              |                  |   |   |    |      |
|      | tes. |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CIP9 | As   | Users must   | Detail Pending   |   | D | CI |      |
|      | an   | be able to   |                  |   | e | P- |      |
|      | Ada  | view a list  |                  |   | t | 16 |      |
|      | hol  | of           |                  |   | a | 94 |      |
|      | der, | governance   |                  |   | i |    |      |
|      |      | actions with |                  |   | l |    |      |
|      | I    | their        |                  |   | P |    |      |
|      | want | current      |                  |   | e |    |      |
|      | to   | status.      |                  |   | n |    |      |
|      | view |              |                  |   | d |    |      |
|      | the  | The status   |                  |   | i |    |      |
|      | st   | must include |                  |   | n |    |      |
|      | atus | stages like  |                  |   | g |    |      |
|      | of   | submission,  |                  |   |   |    |      |
|      | go   | voting,      |                  |   |   |    |      |
|      | vern | r            |                  |   |   |    |      |
|      | ance | atification, |                  |   |   |    |      |
|      | acti | timeline.    |                  |   |   |    |      |
|      | ons, |              |                  |   |   |    |      |
|      |      | The system   |                  |   |   |    |      |
|      | So   | must provide |                  |   |   |    |      |
|      | that | real-time    |                  |   |   |    |      |
|      | I am | updates on   |                  |   |   |    |      |
|      | info | the status.  |                  |   |   |    |      |
|      | rmed |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | bout |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | proc |              |                  |   |   |    |      |
|      | ess. |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | ADA holders  | Detail Pending   |   |   |    |      |
| IP10 | an   | can select a |                  |   |   |    |      |
|      | Ada  | DRep to      |                  |   |   |    |      |
|      | hol  | delegate     |                  |   |   |    |      |
|      | der, | their voting |                  |   |   |    |      |
|      |      | rights.      |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | want | The          |                  |   |   |    |      |
|      | to   | delegation   |                  |   |   |    |      |
|      | dele | process      |                  |   |   |    |      |
|      | gate | should be    |                  |   |   |    |      |
|      | my   | u            |                  |   |   |    |      |
|      | vo   | ser-friendly |                  |   |   |    |      |
|      | ting | and must be  |                  |   |   |    |      |
|      | ri   | secure.      |                  |   |   |    |      |
|      | ghts |              |                  |   |   |    |      |
|      | to a | The system   |                  |   |   |    |      |
|      | D    | must         |                  |   |   |    |      |
|      | Rep, | confirms     |                  |   |   |    |      |
|      |      | successful   |                  |   |   |    |      |
|      | So   | delegation.  |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | i    |              |                  |   |   |    |      |
|      | nter |              |                  |   |   |    |      |
|      | ests |              |                  |   |   |    |      |
|      | are  |              |                  |   |   |    |      |
|      | rep  |              |                  |   |   |    |      |
|      | rese |              |                  |   |   |    |      |
|      | nted |              |                  |   |   |    |      |
|      | in   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | proc |              |                  |   |   |    |      |
|      | ess. |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | SPOs must    | Detail Pending   |   |   |    |      |
| IP11 | an   | have access  |                  |   |   |    |      |
|      | SPO, | to           |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      | I    | actions for  |                  |   |   |    |      |
|      | want | voting.      |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | par  | SPOs can     |                  |   |   |    |      |
|      | tici | cast their   |                  |   |   |    |      |
|      | pate | votes based  |                  |   |   |    |      |
|      | in   | on the ADA   |                  |   |   |    |      |
|      | the  | staked in    |                  |   |   |    |      |
|      | go   | their pools. |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance | The system   |                  |   |   |    |      |
|      | vot  | accurately   |                  |   |   |    |      |
|      | ing, | reflects the |                  |   |   |    |      |
|      |      | votes of     |                  |   |   |    |      |
|      | So   | SPOs.        |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | co   |              |                  |   |   |    |      |
|      | ntri |              |                  |   |   |    |      |
|      | bute |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | dec  |              |                  |   |   |    |      |
|      | isio |              |                  |   |   |    |      |
|      | n-ma |              |                  |   |   |    |      |
|      | king |              |                  |   |   |    |      |
|      | proc |              |                  |   |   |    |      |
|      | ess. |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CAR  |      |              |                  |   |   |    |      |
| DANO |      |              |                  |   |   |    |      |
| CLI  |      |              |                  |   |   |    |      |
| US   |      |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | When I       | Given that a     |   |   | [[ |      |
| LI01 | an   | provide the  | holder provides  |   |   | L9 |      |
|      | Ada  | off-chain    | the offchain     |   |   | 58 |      |
|      | hol  | text of the  | text of the      |   |   | ]{ |      |
|      | der, | C            | constitution     |   |   | .u |      |
|      |      | onstitution, | then cardo-cli   |   |   | nd |      |
|      | I    | the          | should return    |   |   | er |      |
|      | want | cardano-cli  | the              |   |   | li |      |
|      | to   | should       | corresponding    |   |   | ne |      |
|      | ob   | calculate    | blake2b-256 hash |   |   | }] |      |
|      | tain | and return   |                  |   |   | (h |      |
|      | the  | the          | Given that it is |   |   | tt |      |
|      | hash | c            | the same         |   |   | ps |      |
|      | of   | orresponding | document, the    |   |   | :/ |      |
|      | the  | blake2b-256  | resulting hash   |   |   | /g |      |
|      | o    | hash of the  | should match the |   |   | it |      |
|      | ff-c | document.    | one registered   |   |   | hu |      |
|      | hain |              | on-chain.        |   |   | b. |      |
|      | text |              |                  |   |   | co |      |
|      | of a |              |                  |   |   | m/ |      |
|      | Cons |              |                  |   |   | ca |      |
|      | titu |              |                  |   |   | rd |      |
|      | tion |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      | So   |              |                  |   |   | fo |      |
|      | that |              |                  |   |   | un |      |
|      | I    |              |                  |   |   | da |      |
|      | can  |              |                  |   |   | ti |      |
|      | com  |              |                  |   |   | on |      |
|      | pare |              |                  |   |   | /C |      |
|      | it   |              |                  |   |   | IP |      |
|      | aga  |              |                  |   |   | s/ |      |
|      | inst |              |                  |   |   | bl |      |
|      | the  |              |                  |   |   | ob |      |
|      | hash |              |                  |   |   | /d |      |
|      | re   |              |                  |   |   | 6c |      |
|      | gist |              |                  |   |   | 5a |      |
|      | ered |              |                  |   |   | d3 |      |
|      | on-c |              |                  |   |   | a7 |      |
|      | hain |              |                  |   |   | 7b |      |
|      | to   |              |                  |   |   | 46 |      |
|      | ve   |              |                  |   |   | 84 |      |
|      | rify |              |                  |   |   | bc |      |
|      | its  |              |                  |   |   | 19 |      |
|      | a    |              |                  |   |   | f3 |      |
|      | uthe |              |                  |   |   | ca |      |
|      | ntic |              |                  |   |   | fb |      |
|      | ity. |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 95 |      |
|      |      |              |                  |   |   | 8) |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | When I       | Given that a     |   |   | [[ |      |
| LI02 | an   | provide the  | holder provides  |   |   | L9 |      |
|      | Ada  | off-chain    | the offchain     |   |   | 58 |      |
|      | hol  | text of the  | text of the      |   |   | ]{ |      |
|      | der, | C            | constitution     |   |   | .u |      |
|      |      | onstitution, | then cardo-cli   |   |   | nd |      |
|      | I    | the          | should return    |   |   | er |      |
|      | want | cardano-cli  | the              |   |   | li |      |
|      | to   | should       | corresponding    |   |   | ne |      |
|      | gene | calculate    | blake2b-256 hash |   |   | }] |      |
|      | rate | and return   |                  |   |   | (h |      |
|      | the  | the          | Given that it is |   |   | tt |      |
|      | hash | c            | the same         |   |   | ps |      |
|      | of   | orresponding | document, the    |   |   | :/ |      |
|      | the  | blake2b-256  | resulting hash   |   |   | /g |      |
|      | o    | hash of the  | should match the |   |   | it |      |
|      | ff-c | document.    | one registered   |   |   | hu |      |
|      | hain |              | on-chain.        |   |   | b. |      |
|      | text |              |                  |   |   | co |      |
|      | for  |              |                  |   |   | m/ |      |
|      | a    |              |                  |   |   | ca |      |
|      | prop |              |                  |   |   | rd |      |
|      | osed |              |                  |   |   | an |      |
|      | Cons |              |                  |   |   | o- |      |
|      | titu |              |                  |   |   | fo |      |
|      | tion |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      | So   |              |                  |   |   | ti |      |
|      | that |              |                  |   |   | on |      |
|      | the  |              |                  |   |   | /C |      |
|      | hash |              |                  |   |   | IP |      |
|      | can  |              |                  |   |   | s/ |      |
|      | be   |              |                  |   |   | bl |      |
|      | util |              |                  |   |   | ob |      |
|      | ized |              |                  |   |   | /d |      |
|      | in a |              |                  |   |   | 6c |      |
|      | go   |              |                  |   |   | 5a |      |
|      | vern |              |                  |   |   | d3 |      |
|      | ance |              |                  |   |   | a7 |      |
|      | act  |              |                  |   |   | 7b |      |
|      | ion. |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 95 |      |
|      |      |              |                  |   |   | 8) |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As a | [The feature | Typing           |   |   | [  |      |
| LI03 | p    | im           | [cardano-cli     |   |   | [L |      |
|      | oten | plementation | conway           |   |   | 96 |      |
|      | tial | should       | governance       |   |   | 6] |      |
|      | Co   | include a    | committee        |   |   | {. |      |
|      | nsti | new          | key-gen-cold     |   |   | un |      |
|      | tuti | command:\    | with accepted    |   |   | de |      |
|      | onal | \            | input parameters |   |   | rl |      |
|      | C    | cardano-cli  | generates a COLD |   |   | in |      |
|      | ommi | conway       | key pair. If a   |   |   | e} |      |
|      | ttee | governance   | parameter or the |   |   | ]( |      |
|      | mem  | committee    | command format   |   |   | ht |      |
|      | ber, | key-gen-     | is incorrect an  |   |   | tp |      |
|      |      | cold]{.mark} | error is         |   |   | s: |      |
|      | I    |              | raised]{.mark}   |   |   | // |      |
|      | want |              |                  |   |   | gi |      |
|      | to   |              |                  |   |   | th |      |
|      | gene |              |                  |   |   | ub |      |
|      | rate |              |                  |   |   | .c |      |
|      | COLD |              |                  |   |   | om |      |
|      | key  |              |                  |   |   | /c |      |
|      | pair |              |                  |   |   | ar |      |
|      |      |              |                  |   |   | da |      |
|      | So   |              |                  |   |   | no |      |
|      | that |              |                  |   |   | -f |      |
|      | I    |              |                  |   |   | ou |      |
|      | can  |              |                  |   |   | nd |      |
|      | be   |              |                  |   |   | at |      |
|      | prop |              |                  |   |   | io |      |
|      | osed |              |                  |   |   | n/ |      |
|      | for  |              |                  |   |   | CI |      |
|      | the  |              |                  |   |   | Ps |      |
|      | C    |              |                  |   |   | /b |      |
|      | ommi |              |                  |   |   | lo |      |
|      | ttee |              |                  |   |   | b/ |      |
|      | in a |              |                  |   |   | d6 |      |
|      | Go   |              |                  |   |   | c5 |      |
|      | vern |              |                  |   |   | ad |      |
|      | ance |              |                  |   |   | 3a |      |
|      | ac   |              |                  |   |   | 77 |      |
|      | tion |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 68 |      |
|      |      |              |                  |   |   | 4b |      |
|      |      |              |                  |   |   | c1 |      |
|      |      |              |                  |   |   | 9f |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | af |      |
|      |      |              |                  |   |   | b7 |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | 86 |      |
|      |      |              |                  |   |   | a6 |      |
|      |      |              |                  |   |   | 7c |      |
|      |      |              |                  |   |   | 9a |      |
|      |      |              |                  |   |   | 31 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C3 |      |
|      |      |              |                  |   |   | 3- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C5 |      |
|      |      |              |                  |   |   | 2) |      |
|      |      |              |                  |   |   |    |      |
|      |      |              |                  |   |   | [[ |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 93 |      |
|      |      |              |                  |   |   | ]{ |      |
|      |      |              |                  |   |   | .u |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | 6c |      |
|      |      |              |                  |   |   | 5a |      |
|      |      |              |                  |   |   | d3 |      |
|      |      |              |                  |   |   | a7 |      |
|      |      |              |                  |   |   | 7b |      |
|      |      |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Includes a   | Typing           |   |   | [  |      |
|      |      | c            | [cardano-cli     |   |   | [L |      |
|      |      | orresponding | conway           |   |   | 96 |      |
|      |      | CLI usage    | governance       |   |   | 6] |      |
|      |      | describing   | committee        |   |   | {. |      |
|      |      | the feature, | key-gen-cold     |   |   | un |      |
|      |      | how to use   | ----help         |   |   | de |      |
|      |      | it and the   | displays command |   |   | rl |      |
|      |      | types of the | usage]{.mark}    |   |   | in |      |
|      |      | inputs and   |                  |   |   | e} |      |
|      |      | outputs.     |                  |   |   | ]( |      |
|      |      |              |                  |   |   | ht |      |
|      |      |              |                  |   |   | tp |      |
|      |      |              |                  |   |   | s: |      |
|      |      |              |                  |   |   | // |      |
|      |      |              |                  |   |   | gi |      |
|      |      |              |                  |   |   | th |      |
|      |      |              |                  |   |   | ub |      |
|      |      |              |                  |   |   | .c |      |
|      |      |              |                  |   |   | om |      |
|      |      |              |                  |   |   | /c |      |
|      |      |              |                  |   |   | ar |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | no |      |
|      |      |              |                  |   |   | -f |      |
|      |      |              |                  |   |   | ou |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | at |      |
|      |      |              |                  |   |   | io |      |
|      |      |              |                  |   |   | n/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | Ps |      |
|      |      |              |                  |   |   | /b |      |
|      |      |              |                  |   |   | lo |      |
|      |      |              |                  |   |   | b/ |      |
|      |      |              |                  |   |   | d6 |      |
|      |      |              |                  |   |   | c5 |      |
|      |      |              |                  |   |   | ad |      |
|      |      |              |                  |   |   | 3a |      |
|      |      |              |                  |   |   | 77 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 68 |      |
|      |      |              |                  |   |   | 4b |      |
|      |      |              |                  |   |   | c1 |      |
|      |      |              |                  |   |   | 9f |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | af |      |
|      |      |              |                  |   |   | b7 |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | 86 |      |
|      |      |              |                  |   |   | a6 |      |
|      |      |              |                  |   |   | 7c |      |
|      |      |              |                  |   |   | 9a |      |
|      |      |              |                  |   |   | 31 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C3 |      |
|      |      |              |                  |   |   | 3- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C5 |      |
|      |      |              |                  |   |   | 2) |      |
|      |      |              |                  |   |   |    |      |
|      |      |              |                  |   |   | [[ |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 93 |      |
|      |      |              |                  |   |   | ]{ |      |
|      |      |              |                  |   |   | .u |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | 6c |      |
|      |      |              |                  |   |   | 5a |      |
|      |      |              |                  |   |   | d3 |      |
|      |      |              |                  |   |   | a7 |      |
|      |      |              |                  |   |   | 7b |      |
|      |      |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The command  | Both flags are   |   |   | [  |      |
|      |      | must accept  | mandatory and    |   |   | [L |      |
|      |      | two flags    | each produces    |   |   | 96 |      |
|      |      |              | the              |   |   | 6] |      |
|      |      | \--co        | corresponding    |   |   | {. |      |
|      |      | ld-verificat | verification or  |   |   | un |      |
|      |      | ion-key-file | signing key file |   |   | de |      |
|      |      |              |                  |   |   | rl |      |
|      |      | \--cold-sign |                  |   |   | in |      |
|      |      | ing-key-file |                  |   |   | e} |      |
|      |      |              |                  |   |   | ]( |      |
|      |      |              |                  |   |   | ht |      |
|      |      |              |                  |   |   | tp |      |
|      |      |              |                  |   |   | s: |      |
|      |      |              |                  |   |   | // |      |
|      |      |              |                  |   |   | gi |      |
|      |      |              |                  |   |   | th |      |
|      |      |              |                  |   |   | ub |      |
|      |      |              |                  |   |   | .c |      |
|      |      |              |                  |   |   | om |      |
|      |      |              |                  |   |   | /c |      |
|      |      |              |                  |   |   | ar |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | no |      |
|      |      |              |                  |   |   | -f |      |
|      |      |              |                  |   |   | ou |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | at |      |
|      |      |              |                  |   |   | io |      |
|      |      |              |                  |   |   | n/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | Ps |      |
|      |      |              |                  |   |   | /b |      |
|      |      |              |                  |   |   | lo |      |
|      |      |              |                  |   |   | b/ |      |
|      |      |              |                  |   |   | d6 |      |
|      |      |              |                  |   |   | c5 |      |
|      |      |              |                  |   |   | ad |      |
|      |      |              |                  |   |   | 3a |      |
|      |      |              |                  |   |   | 77 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 68 |      |
|      |      |              |                  |   |   | 4b |      |
|      |      |              |                  |   |   | c1 |      |
|      |      |              |                  |   |   | 9f |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | af |      |
|      |      |              |                  |   |   | b7 |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | 86 |      |
|      |      |              |                  |   |   | a6 |      |
|      |      |              |                  |   |   | 7c |      |
|      |      |              |                  |   |   | 9a |      |
|      |      |              |                  |   |   | 31 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C3 |      |
|      |      |              |                  |   |   | 3- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C5 |      |
|      |      |              |                  |   |   | 2) |      |
|      |      |              |                  |   |   |    |      |
|      |      |              |                  |   |   | [[ |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 93 |      |
|      |      |              |                  |   |   | ]{ |      |
|      |      |              |                  |   |   | .u |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | 6c |      |
|      |      |              |                  |   |   | 5a |      |
|      |      |              |                  |   |   | d3 |      |
|      |      |              |                  |   |   | a7 |      |
|      |      |              |                  |   |   | 7b |      |
|      |      |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Given that the   |   |   | [  |      |
|      |      | generated    | user specifies a |   |   | [L |      |
|      |      | key pair     | valid path and   |   |   | 96 |      |
|      |      | should be    | file name, Then  |   |   | 6] |      |
|      |      | stored in    | the keys are     |   |   | {. |      |
|      |      | the          | saved on that    |   |   | un |      |
|      |      | specified    | file and         |   |   | de |      |
|      |      | fi           | location.        |   |   | rl |      |
|      |      | les:]{.mark} |                  |   |   | in |      |
|      |      |              |                  |   |   | e} |      |
|      |      | [the         |                  |   |   | ]( |      |
|      |      | verification |                  |   |   | ht |      |
|      |      | key is saved |                  |   |   | tp |      |
|      |      | in the file  |                  |   |   | s: |      |
|      |      | specified    |                  |   |   | // |      |
|      |      | by]{.mark}   |                  |   |   | gi |      |
|      |      | \--co        |                  |   |   | th |      |
|      |      | ld-verificat |                  |   |   | ub |      |
|      |      | ion-key-file |                  |   |   | .c |      |
|      |      |              |                  |   |   | om |      |
|      |      | [the signing |                  |   |   | /c |      |
|      |      | key saved in |                  |   |   | ar |      |
|      |      | the file     |                  |   |   | da |      |
|      |      | specified    |                  |   |   | no |      |
|      |      | by]{.mark}   |                  |   |   | -f |      |
|      |      |              |                  |   |   | ou |      |
|      |      | \--cold-sign |                  |   |   | nd |      |
|      |      | ing-key-file |                  |   |   | at |      |
|      |      |              |                  |   |   | io |      |
|      |      |              |                  |   |   | n/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | Ps |      |
|      |      |              |                  |   |   | /b |      |
|      |      |              |                  |   |   | lo |      |
|      |      |              |                  |   |   | b/ |      |
|      |      |              |                  |   |   | d6 |      |
|      |      |              |                  |   |   | c5 |      |
|      |      |              |                  |   |   | ad |      |
|      |      |              |                  |   |   | 3a |      |
|      |      |              |                  |   |   | 77 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 68 |      |
|      |      |              |                  |   |   | 4b |      |
|      |      |              |                  |   |   | c1 |      |
|      |      |              |                  |   |   | 9f |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | af |      |
|      |      |              |                  |   |   | b7 |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | 86 |      |
|      |      |              |                  |   |   | a6 |      |
|      |      |              |                  |   |   | 7c |      |
|      |      |              |                  |   |   | 9a |      |
|      |      |              |                  |   |   | 31 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C3 |      |
|      |      |              |                  |   |   | 3- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C5 |      |
|      |      |              |                  |   |   | 2) |      |
|      |      |              |                  |   |   |    |      |
|      |      |              |                  |   |   | [[ |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 93 |      |
|      |      |              |                  |   |   | ]{ |      |
|      |      |              |                  |   |   | .u |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | 6c |      |
|      |      |              |                  |   |   | 5a |      |
|      |      |              |                  |   |   | d3 |      |
|      |      |              |                  |   |   | a7 |      |
|      |      |              |                  |   |   | 7b |      |
|      |      |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Given that the   |   |   | [  |      |
|      |      | generated    | cli has created  |   |   | [L |      |
|      |      | keys should  | the verification |   |   | 96 |      |
|      |      | adhere to    | and signing      |   |   | 6] |      |
|      |      | text         | keys, then these |   |   | {. |      |
|      |      | envelope     | conform to the   |   |   | un |      |
|      |      | format used  | text envelope    |   |   | de |      |
|      |      | for other    | format used      |   |   | rl |      |
|      |      | credent      | consisting of a  |   |   | in |      |
|      |      | ials]{.mark} | json object with |   |   | e} |      |
|      |      |              | type,            |   |   | ]( |      |
|      |      |              | description and  |   |   | ht |      |
|      |      |              | cborhex fields.  |   |   | tp |      |
|      |      |              |                  |   |   | s: |      |
|      |      |              |                  |   |   | // |      |
|      |      |              |                  |   |   | gi |      |
|      |      |              |                  |   |   | th |      |
|      |      |              |                  |   |   | ub |      |
|      |      |              |                  |   |   | .c |      |
|      |      |              |                  |   |   | om |      |
|      |      |              |                  |   |   | /c |      |
|      |      |              |                  |   |   | ar |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | no |      |
|      |      |              |                  |   |   | -f |      |
|      |      |              |                  |   |   | ou |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | at |      |
|      |      |              |                  |   |   | io |      |
|      |      |              |                  |   |   | n/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | Ps |      |
|      |      |              |                  |   |   | /b |      |
|      |      |              |                  |   |   | lo |      |
|      |      |              |                  |   |   | b/ |      |
|      |      |              |                  |   |   | d6 |      |
|      |      |              |                  |   |   | c5 |      |
|      |      |              |                  |   |   | ad |      |
|      |      |              |                  |   |   | 3a |      |
|      |      |              |                  |   |   | 77 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 68 |      |
|      |      |              |                  |   |   | 4b |      |
|      |      |              |                  |   |   | c1 |      |
|      |      |              |                  |   |   | 9f |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | af |      |
|      |      |              |                  |   |   | b7 |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | 86 |      |
|      |      |              |                  |   |   | a6 |      |
|      |      |              |                  |   |   | 7c |      |
|      |      |              |                  |   |   | 9a |      |
|      |      |              |                  |   |   | 31 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C3 |      |
|      |      |              |                  |   |   | 3- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C5 |      |
|      |      |              |                  |   |   | 2) |      |
|      |      |              |                  |   |   |    |      |
|      |      |              |                  |   |   | [[ |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 93 |      |
|      |      |              |                  |   |   | ]{ |      |
|      |      |              |                  |   |   | .u |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | 6c |      |
|      |      |              |                  |   |   | 5a |      |
|      |      |              |                  |   |   | d3 |      |
|      |      |              |                  |   |   | a7 |      |
|      |      |              |                  |   |   | 7b |      |
|      |      |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The signing | Given that the   |   |   | [  |      |
|      |      | key text     | signing key is   |   |   | [L |      |
|      |      | envelope     | saved on a text  |   |   | 96 |      |
|      |      | contains the | envelope format, |   |   | 6] |      |
|      |      | correct      | the type and     |   |   | {. |      |
|      |      | type,        | description      |   |   | un |      |
|      |      | description, | fields are:      |   |   | de |      |
|      |      | and CBOR     |                  |   |   | rl |      |
|      |      | va           | [Type            |   |   | in |      |
|      |      | lue.]{.mark} | \"Constit        |   |   | e} |      |
|      |      |              | utionalCommittee |   |   | ]( |      |
|      |      | [Type        | ColdSigningKey_e |   |   | ht |      |
|      |      | \"Constit    | d25519\"]{.mark} |   |   | tp |      |
|      |      | utionalCommi |                  |   |   | s: |      |
|      |      | tteeColdSign | [Des             |   |   | // |      |
|      |      | ingKey_ed255 | cription]{.mark} |   |   | gi |      |
|      |      | 19\"]{.mark} |                  |   |   | th |      |
|      |      |              | [                |   |   | ub |      |
|      |      | [Descrip     | \"Constitutional |   |   | .c |      |
|      |      | tion]{.mark} | Committee Cold   |   |   | om |      |
|      |      |              | Signing          |   |   | /c |      |
|      |      | [\"Co        | Key\"]{.mark}    |   |   | ar |      |
|      |      | nstitutional |                  |   |   | da |      |
|      |      | Committee    |                  |   |   | no |      |
|      |      | Cold Signing |                  |   |   | -f |      |
|      |      | K            |                  |   |   | ou |      |
|      |      | ey\"]{.mark} |                  |   |   | nd |      |
|      |      |              |                  |   |   | at |      |
|      |      |              |                  |   |   | io |      |
|      |      |              |                  |   |   | n/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | Ps |      |
|      |      |              |                  |   |   | /b |      |
|      |      |              |                  |   |   | lo |      |
|      |      |              |                  |   |   | b/ |      |
|      |      |              |                  |   |   | d6 |      |
|      |      |              |                  |   |   | c5 |      |
|      |      |              |                  |   |   | ad |      |
|      |      |              |                  |   |   | 3a |      |
|      |      |              |                  |   |   | 77 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 68 |      |
|      |      |              |                  |   |   | 4b |      |
|      |      |              |                  |   |   | c1 |      |
|      |      |              |                  |   |   | 9f |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | af |      |
|      |      |              |                  |   |   | b7 |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | 86 |      |
|      |      |              |                  |   |   | a6 |      |
|      |      |              |                  |   |   | 7c |      |
|      |      |              |                  |   |   | 9a |      |
|      |      |              |                  |   |   | 31 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C3 |      |
|      |      |              |                  |   |   | 3- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C5 |      |
|      |      |              |                  |   |   | 2) |      |
|      |      |              |                  |   |   |    |      |
|      |      |              |                  |   |   | [[ |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 93 |      |
|      |      |              |                  |   |   | ]{ |      |
|      |      |              |                  |   |   | .u |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | 6c |      |
|      |      |              |                  |   |   | 5a |      |
|      |      |              |                  |   |   | d3 |      |
|      |      |              |                  |   |   | a7 |      |
|      |      |              |                  |   |   | 7b |      |
|      |      |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The          | Given that the   |   |   | [  |      |
|      |      | verification | verification key |   |   | [L |      |
|      |      | key text     | is saved on a    |   |   | 96 |      |
|      |      | envelope     | text envelope    |   |   | 6] |      |
|      |      | has:         | format, the type |   |   | {. |      |
|      |      |              | and description  |   |   | un |      |
|      |      | Type         | fields are:      |   |   | de |      |
|      |      | \"CCons      |                  |   |   | rl |      |
|      |      | titutionalCo | Type             |   |   | in |      |
|      |      | mmitteeColdV | [\"CConstitution |   |   | e} |      |
|      |      | erificationK | alCommitteeColdV |   |   | ]( |      |
|      |      | ey_ed25519\" | erificationKey_e |   |   | ht |      |
|      |      |              | d25519\"]{.mark} |   |   | tp |      |
|      |      | Description  |                  |   |   | s: |      |
|      |      |              | Description      |   |   | // |      |
|      |      | \"Co         |                  |   |   | gi |      |
|      |      | nstitutional | [                |   |   | th |      |
|      |      | Committee    | \"Constitutional |   |   | ub |      |
|      |      | Cold         | Committee Cold   |   |   | .c |      |
|      |      | Verification | Verification     |   |   | om |      |
|      |      | Key\"        | Key\"]{.mark}    |   |   | /c |      |
|      |      |              |                  |   |   | ar |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | no |      |
|      |      |              |                  |   |   | -f |      |
|      |      |              |                  |   |   | ou |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | at |      |
|      |      |              |                  |   |   | io |      |
|      |      |              |                  |   |   | n/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | Ps |      |
|      |      |              |                  |   |   | /b |      |
|      |      |              |                  |   |   | lo |      |
|      |      |              |                  |   |   | b/ |      |
|      |      |              |                  |   |   | d6 |      |
|      |      |              |                  |   |   | c5 |      |
|      |      |              |                  |   |   | ad |      |
|      |      |              |                  |   |   | 3a |      |
|      |      |              |                  |   |   | 77 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 68 |      |
|      |      |              |                  |   |   | 4b |      |
|      |      |              |                  |   |   | c1 |      |
|      |      |              |                  |   |   | 9f |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | af |      |
|      |      |              |                  |   |   | b7 |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | 86 |      |
|      |      |              |                  |   |   | a6 |      |
|      |      |              |                  |   |   | 7c |      |
|      |      |              |                  |   |   | 9a |      |
|      |      |              |                  |   |   | 31 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C3 |      |
|      |      |              |                  |   |   | 3- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C5 |      |
|      |      |              |                  |   |   | 2) |      |
|      |      |              |                  |   |   |    |      |
|      |      |              |                  |   |   | [[ |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 93 |      |
|      |      |              |                  |   |   | ]{ |      |
|      |      |              |                  |   |   | .u |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | 6c |      |
|      |      |              |                  |   |   | 5a |      |
|      |      |              |                  |   |   | d3 |      |
|      |      |              |                  |   |   | a7 |      |
|      |      |              |                  |   |   | 7b |      |
|      |      |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Failing to   | Given the user   |   |   | [  |      |
|      |      | provide a    | has not inputed  |   |   | [L |      |
|      |      | file name    | either           |   |   | 96 |      |
|      |      | for any of   | [\--co           |   |   | 6] |      |
|      |      |              | ld-verification- |   |   | {. |      |
|      |      | \--co        | key-file]{.mark} |   |   | un |      |
|      |      | ld-verificat | OR               |   |   | de |      |
|      |      | ion-key-file |                  |   |   | rl |      |
|      |      |              | [                |   |   | in |      |
|      |      | \--cold-sign | \--cold-signing- |   |   | e} |      |
|      |      | ing-key-file | key-file]{.mark} |   |   | ]( |      |
|      |      |              | parameters THEN  |   |   | ht |      |
|      |      | fails with   | the command      |   |   | tp |      |
|      |      | an           | fails and        |   |   | s: |      |
|      |      | appropriate  | returns an error |   |   | // |      |
|      |      | error        | to the users     |   |   | gi |      |
|      |      | message.     | informing them   |   |   | th |      |
|      |      |              | to fill those    |   |   | ub |      |
|      |      |              | parameters in.   |   |   | .c |      |
|      |      |              | The error        |   |   | om |      |
|      |      |              | message should   |   |   | /c |      |
|      |      |              | prompt the user  |   |   | ar |      |
|      |      |              | to consult the   |   |   | da |      |
|      |      |              | command usage    |   |   | no |      |
|      |      |              | (\--help)        |   |   | -f |      |
|      |      |              |                  |   |   | ou |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | at |      |
|      |      |              |                  |   |   | io |      |
|      |      |              |                  |   |   | n/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | Ps |      |
|      |      |              |                  |   |   | /b |      |
|      |      |              |                  |   |   | lo |      |
|      |      |              |                  |   |   | b/ |      |
|      |      |              |                  |   |   | d6 |      |
|      |      |              |                  |   |   | c5 |      |
|      |      |              |                  |   |   | ad |      |
|      |      |              |                  |   |   | 3a |      |
|      |      |              |                  |   |   | 77 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 68 |      |
|      |      |              |                  |   |   | 4b |      |
|      |      |              |                  |   |   | c1 |      |
|      |      |              |                  |   |   | 9f |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | af |      |
|      |      |              |                  |   |   | b7 |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | 86 |      |
|      |      |              |                  |   |   | a6 |      |
|      |      |              |                  |   |   | 7c |      |
|      |      |              |                  |   |   | 9a |      |
|      |      |              |                  |   |   | 31 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C3 |      |
|      |      |              |                  |   |   | 3- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C5 |      |
|      |      |              |                  |   |   | 2) |      |
|      |      |              |                  |   |   |    |      |
|      |      |              |                  |   |   | [[ |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 93 |      |
|      |      |              |                  |   |   | ]{ |      |
|      |      |              |                  |   |   | .u |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | 6c |      |
|      |      |              |                  |   |   | 5a |      |
|      |      |              |                  |   |   | d3 |      |
|      |      |              |                  |   |   | a7 |      |
|      |      |              |                  |   |   | 7b |      |
|      |      |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [The feature | Given that a     |   |   | [  |      |
| LI04 | p    | im           | potential        |   |   | [L |      |
|      | oten | plementation | constitutional   |   |   | 96 |      |
|      | tial | should       | committee member |   |   | 6] |      |
|      | Co   | include a    | has entered the  |   |   | {. |      |
|      | nsti | new          | [cardano-cli     |   |   | un |      |
|      | tuti | command:\    | conway           |   |   | de |      |
|      | onal | \            | governance       |   |   | rl |      |
|      | C    | cardano-cli  | committee        |   |   | in |      |
|      | ommi | conway       | key-gen-hot      |   |   | e} |      |
|      | ttee | governance   | command with all |   |   | ]( |      |
|      | mem  | committee    | the required and |   |   | ht |      |
|      | ber, | key-gen      | correct          |   |   | tp |      |
|      |      | -hot]{.mark} | pa               |   |   | s: |      |
|      | I    |              | rameters]{.mark} |   |   | // |      |
|      | want |              | then the command |   |   | gi |      |
|      | to   |              | is executed      |   |   | th |      |
|      | gene |              | successfully and |   |   | ub |      |
|      | rate |              | a HOT key pair   |   |   | .c |      |
|      | HOT  |              | is generated.    |   |   | om |      |
|      | key  |              |                  |   |   | /c |      |
|      | pair |              | [If a parameter  |   |   | ar |      |
|      |      |              | or the command   |   |   | da |      |
|      | So   |              | format is        |   |   | no |      |
|      | that |              | incorrect an     |   |   | -f |      |
|      | I    |              | error is         |   |   | ou |      |
|      | can  |              | raised]{.mark}   |   |   | nd |      |
|      | a    |              |                  |   |   | at |      |
|      | utho |              |                  |   |   | io |      |
|      | rise |              |                  |   |   | n/ |      |
|      | the  |              |                  |   |   | CI |      |
|      | Hot  |              |                  |   |   | Ps |      |
|      | key  |              |                  |   |   | /b |      |
|      | to   |              |                  |   |   | lo |      |
|      | sign |              |                  |   |   | b/ |      |
|      | v    |              |                  |   |   | d6 |      |
|      | otes |              |                  |   |   | c5 |      |
|      | on   |              |                  |   |   | ad |      |
|      | be   |              |                  |   |   | 3a |      |
|      | half |              |                  |   |   | 77 |      |
|      | of   |              |                  |   |   | b4 |      |
|      | the  |              |                  |   |   | 68 |      |
|      | Cold |              |                  |   |   | 4b |      |
|      | key  |              |                  |   |   | c1 |      |
|      |      |              |                  |   |   | 9f |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | af |      |
|      |      |              |                  |   |   | b7 |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | 86 |      |
|      |      |              |                  |   |   | a6 |      |
|      |      |              |                  |   |   | 7c |      |
|      |      |              |                  |   |   | 9a |      |
|      |      |              |                  |   |   | 31 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C3 |      |
|      |      |              |                  |   |   | 3- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C5 |      |
|      |      |              |                  |   |   | 2) |      |
|      |      |              |                  |   |   |    |      |
|      |      |              |                  |   |   | [[ |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 93 |      |
|      |      |              |                  |   |   | ]{ |      |
|      |      |              |                  |   |   | .u |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | 6c |      |
|      |      |              |                  |   |   | 5a |      |
|      |      |              |                  |   |   | d3 |      |
|      |      |              |                  |   |   | a7 |      |
|      |      |              |                  |   |   | 7b |      |
|      |      |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Includes a   | Typing           |   | D | [  |      |
|      |      | c            | [cardano-cli     |   | e | [L |      |
|      |      | orresponding | conway           |   | t | 96 |      |
|      |      | CLI usage    | governance       |   | a | 6] |      |
|      |      | describing   | committee        |   | i | {. |      |
|      |      | the feature, | key-gen-hot      |   | l | un |      |
|      |      | how to use   | displays command |   | P | de |      |
|      |      | it and the   | usage]{.mark}    |   | e | rl |      |
|      |      | types of the |                  |   | n | in |      |
|      |      | inputs and   |                  |   | d | e} |      |
|      |      | outputs.     |                  |   | i | ]( |      |
|      |      |              |                  |   | n | ht |      |
|      |      |              |                  |   | g | tp |      |
|      |      |              |                  |   |   | s: |      |
|      |      |              |                  |   |   | // |      |
|      |      |              |                  |   |   | gi |      |
|      |      |              |                  |   |   | th |      |
|      |      |              |                  |   |   | ub |      |
|      |      |              |                  |   |   | .c |      |
|      |      |              |                  |   |   | om |      |
|      |      |              |                  |   |   | /c |      |
|      |      |              |                  |   |   | ar |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | no |      |
|      |      |              |                  |   |   | -f |      |
|      |      |              |                  |   |   | ou |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | at |      |
|      |      |              |                  |   |   | io |      |
|      |      |              |                  |   |   | n/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | Ps |      |
|      |      |              |                  |   |   | /b |      |
|      |      |              |                  |   |   | lo |      |
|      |      |              |                  |   |   | b/ |      |
|      |      |              |                  |   |   | d6 |      |
|      |      |              |                  |   |   | c5 |      |
|      |      |              |                  |   |   | ad |      |
|      |      |              |                  |   |   | 3a |      |
|      |      |              |                  |   |   | 77 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 68 |      |
|      |      |              |                  |   |   | 4b |      |
|      |      |              |                  |   |   | c1 |      |
|      |      |              |                  |   |   | 9f |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | af |      |
|      |      |              |                  |   |   | b7 |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | 86 |      |
|      |      |              |                  |   |   | a6 |      |
|      |      |              |                  |   |   | 7c |      |
|      |      |              |                  |   |   | 9a |      |
|      |      |              |                  |   |   | 31 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C3 |      |
|      |      |              |                  |   |   | 3- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C5 |      |
|      |      |              |                  |   |   | 2) |      |
|      |      |              |                  |   |   |    |      |
|      |      |              |                  |   |   | [[ |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 93 |      |
|      |      |              |                  |   |   | ]{ |      |
|      |      |              |                  |   |   | .u |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | 6c |      |
|      |      |              |                  |   |   | 5a |      |
|      |      |              |                  |   |   | d3 |      |
|      |      |              |                  |   |   | a7 |      |
|      |      |              |                  |   |   | 7b |      |
|      |      |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The command  | Both flags are   |   | D | [  |      |
|      |      | must accept  | mandatory and    |   | e | [L |      |
|      |      | two flags    | each produces    |   | t | 96 |      |
|      |      |              | the              |   | a | 6] |      |
|      |      | \--verificat | corresponding    |   | i | {. |      |
|      |      | ion-key-file | verification or  |   | l | un |      |
|      |      |              | signing key file |   | P | de |      |
|      |      | \--sign      |                  |   | e | rl |      |
|      |      | ing-key-file |                  |   | n | in |      |
|      |      |              |                  |   | d | e} |      |
|      |      |              |                  |   | i | ]( |      |
|      |      |              |                  |   | n | ht |      |
|      |      |              |                  |   | g | tp |      |
|      |      |              |                  |   |   | s: |      |
|      |      |              |                  |   |   | // |      |
|      |      |              |                  |   |   | gi |      |
|      |      |              |                  |   |   | th |      |
|      |      |              |                  |   |   | ub |      |
|      |      |              |                  |   |   | .c |      |
|      |      |              |                  |   |   | om |      |
|      |      |              |                  |   |   | /c |      |
|      |      |              |                  |   |   | ar |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | no |      |
|      |      |              |                  |   |   | -f |      |
|      |      |              |                  |   |   | ou |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | at |      |
|      |      |              |                  |   |   | io |      |
|      |      |              |                  |   |   | n/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | Ps |      |
|      |      |              |                  |   |   | /b |      |
|      |      |              |                  |   |   | lo |      |
|      |      |              |                  |   |   | b/ |      |
|      |      |              |                  |   |   | d6 |      |
|      |      |              |                  |   |   | c5 |      |
|      |      |              |                  |   |   | ad |      |
|      |      |              |                  |   |   | 3a |      |
|      |      |              |                  |   |   | 77 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 68 |      |
|      |      |              |                  |   |   | 4b |      |
|      |      |              |                  |   |   | c1 |      |
|      |      |              |                  |   |   | 9f |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | af |      |
|      |      |              |                  |   |   | b7 |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | 86 |      |
|      |      |              |                  |   |   | a6 |      |
|      |      |              |                  |   |   | 7c |      |
|      |      |              |                  |   |   | 9a |      |
|      |      |              |                  |   |   | 31 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C3 |      |
|      |      |              |                  |   |   | 3- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C5 |      |
|      |      |              |                  |   |   | 2) |      |
|      |      |              |                  |   |   |    |      |
|      |      |              |                  |   |   | [[ |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 93 |      |
|      |      |              |                  |   |   | ]{ |      |
|      |      |              |                  |   |   | .u |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | 6c |      |
|      |      |              |                  |   |   | 5a |      |
|      |      |              |                  |   |   | d3 |      |
|      |      |              |                  |   |   | a7 |      |
|      |      |              |                  |   |   | 7b |      |
|      |      |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Given that the   |   |   | [  |      |
|      |      | generated    | user specifies a |   |   | [L |      |
|      |      | key pair     | valid path and   |   |   | 96 |      |
|      |      | should be    | file name, Then  |   |   | 6] |      |
|      |      | stored in    | the keys are     |   |   | {. |      |
|      |      | the          | saved on that    |   |   | un |      |
|      |      | specified    | file and         |   |   | de |      |
|      |      | fi           | location.        |   |   | rl |      |
|      |      | les:]{.mark} |                  |   |   | in |      |
|      |      |              |                  |   |   | e} |      |
|      |      | [the         |                  |   |   | ]( |      |
|      |      | verification |                  |   |   | ht |      |
|      |      | key saved in |                  |   |   | tp |      |
|      |      | the file     |                  |   |   | s: |      |
|      |      | specified    |                  |   |   | // |      |
|      |      | by]{.mark}   |                  |   |   | gi |      |
|      |      |              |                  |   |   | th |      |
|      |      | [\--verif    |                  |   |   | ub |      |
|      |      | ication-key- |                  |   |   | .c |      |
|      |      | file]{.mark} |                  |   |   | om |      |
|      |      |              |                  |   |   | /c |      |
|      |      | [the signing |                  |   |   | ar |      |
|      |      | key saved in |                  |   |   | da |      |
|      |      | the file     |                  |   |   | no |      |
|      |      | specified    |                  |   |   | -f |      |
|      |      | by]{.mark}   |                  |   |   | ou |      |
|      |      |              |                  |   |   | nd |      |
|      |      | [\--         |                  |   |   | at |      |
|      |      | signing-key- |                  |   |   | io |      |
|      |      | file]{.mark} |                  |   |   | n/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | Ps |      |
|      |      |              |                  |   |   | /b |      |
|      |      |              |                  |   |   | lo |      |
|      |      |              |                  |   |   | b/ |      |
|      |      |              |                  |   |   | d6 |      |
|      |      |              |                  |   |   | c5 |      |
|      |      |              |                  |   |   | ad |      |
|      |      |              |                  |   |   | 3a |      |
|      |      |              |                  |   |   | 77 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 68 |      |
|      |      |              |                  |   |   | 4b |      |
|      |      |              |                  |   |   | c1 |      |
|      |      |              |                  |   |   | 9f |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | af |      |
|      |      |              |                  |   |   | b7 |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | 86 |      |
|      |      |              |                  |   |   | a6 |      |
|      |      |              |                  |   |   | 7c |      |
|      |      |              |                  |   |   | 9a |      |
|      |      |              |                  |   |   | 31 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C3 |      |
|      |      |              |                  |   |   | 3- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C5 |      |
|      |      |              |                  |   |   | 2) |      |
|      |      |              |                  |   |   |    |      |
|      |      |              |                  |   |   | [[ |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 93 |      |
|      |      |              |                  |   |   | ]{ |      |
|      |      |              |                  |   |   | .u |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | 6c |      |
|      |      |              |                  |   |   | 5a |      |
|      |      |              |                  |   |   | d3 |      |
|      |      |              |                  |   |   | a7 |      |
|      |      |              |                  |   |   | 7b |      |
|      |      |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Given that the   |   |   | [  |      |
|      |      | generated    | cli has created  |   |   | [L |      |
|      |      | keys should  | the verification |   |   | 96 |      |
|      |      | adhere to    | and signing      |   |   | 6] |      |
|      |      | text         | keys, then these |   |   | {. |      |
|      |      | envelope     | conform to the   |   |   | un |      |
|      |      | format used  | text envelope    |   |   | de |      |
|      |      | for other    | format used      |   |   | rl |      |
|      |      | credent      | consisting of a  |   |   | in |      |
|      |      | ials]{.mark} | json object with |   |   | e} |      |
|      |      |              | type,            |   |   | ]( |      |
|      |      |              | description and  |   |   | ht |      |
|      |      |              | cbor hex fields. |   |   | tp |      |
|      |      |              |                  |   |   | s: |      |
|      |      |              |                  |   |   | // |      |
|      |      |              |                  |   |   | gi |      |
|      |      |              |                  |   |   | th |      |
|      |      |              |                  |   |   | ub |      |
|      |      |              |                  |   |   | .c |      |
|      |      |              |                  |   |   | om |      |
|      |      |              |                  |   |   | /c |      |
|      |      |              |                  |   |   | ar |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | no |      |
|      |      |              |                  |   |   | -f |      |
|      |      |              |                  |   |   | ou |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | at |      |
|      |      |              |                  |   |   | io |      |
|      |      |              |                  |   |   | n/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | Ps |      |
|      |      |              |                  |   |   | /b |      |
|      |      |              |                  |   |   | lo |      |
|      |      |              |                  |   |   | b/ |      |
|      |      |              |                  |   |   | d6 |      |
|      |      |              |                  |   |   | c5 |      |
|      |      |              |                  |   |   | ad |      |
|      |      |              |                  |   |   | 3a |      |
|      |      |              |                  |   |   | 77 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 68 |      |
|      |      |              |                  |   |   | 4b |      |
|      |      |              |                  |   |   | c1 |      |
|      |      |              |                  |   |   | 9f |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | af |      |
|      |      |              |                  |   |   | b7 |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | 86 |      |
|      |      |              |                  |   |   | a6 |      |
|      |      |              |                  |   |   | 7c |      |
|      |      |              |                  |   |   | 9a |      |
|      |      |              |                  |   |   | 31 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C3 |      |
|      |      |              |                  |   |   | 3- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C5 |      |
|      |      |              |                  |   |   | 2) |      |
|      |      |              |                  |   |   |    |      |
|      |      |              |                  |   |   | [[ |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 93 |      |
|      |      |              |                  |   |   | ]{ |      |
|      |      |              |                  |   |   | .u |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | 6c |      |
|      |      |              |                  |   |   | 5a |      |
|      |      |              |                  |   |   | d3 |      |
|      |      |              |                  |   |   | a7 |      |
|      |      |              |                  |   |   | 7b |      |
|      |      |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The signing | Given that the   |   |   | [  |      |
|      |      | key text     | signing key is   |   |   | [L |      |
|      |      | envelope     | saved on a text  |   |   | 96 |      |
|      |      | contains the | envelope format, |   |   | 6] |      |
|      |      | correct      | the type and     |   |   | {. |      |
|      |      | type,        | description      |   |   | un |      |
|      |      | description, | fields are:      |   |   | de |      |
|      |      | and CBOR     |                  |   |   | rl |      |
|      |      | va           | [Type]{.mark}    |   |   | in |      |
|      |      | lue.]{.mark} | \                |   |   | e} |      |
|      |      |              | "ConstitutionalC |   |   | ]( |      |
|      |      | [Type        | ommitteeColdSign |   |   | ht |      |
|      |      | \"Constit    | ingKey_ed25519\" |   |   | tp |      |
|      |      | utionalCommi |                  |   |   | s: |      |
|      |      | tteeColdSign | [Des             |   |   | // |      |
|      |      | ingKey_ed255 | cription]{.mark} |   |   | gi |      |
|      |      | 19\"]{.mark} |                  |   |   | th |      |
|      |      |              | \"Constitutional |   |   | ub |      |
|      |      | [Descrip     | Committee Cold   |   |   | .c |      |
|      |      | tion]{.mark} | Signing Key\"    |   |   | om |      |
|      |      |              |                  |   |   | /c |      |
|      |      | [\"Co        |                  |   |   | ar |      |
|      |      | nstitutional |                  |   |   | da |      |
|      |      | Committee    |                  |   |   | no |      |
|      |      | Cold Signing |                  |   |   | -f |      |
|      |      | K            |                  |   |   | ou |      |
|      |      | ey\"]{.mark} |                  |   |   | nd |      |
|      |      |              |                  |   |   | at |      |
|      |      |              |                  |   |   | io |      |
|      |      |              |                  |   |   | n/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | Ps |      |
|      |      |              |                  |   |   | /b |      |
|      |      |              |                  |   |   | lo |      |
|      |      |              |                  |   |   | b/ |      |
|      |      |              |                  |   |   | d6 |      |
|      |      |              |                  |   |   | c5 |      |
|      |      |              |                  |   |   | ad |      |
|      |      |              |                  |   |   | 3a |      |
|      |      |              |                  |   |   | 77 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 68 |      |
|      |      |              |                  |   |   | 4b |      |
|      |      |              |                  |   |   | c1 |      |
|      |      |              |                  |   |   | 9f |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | af |      |
|      |      |              |                  |   |   | b7 |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | 86 |      |
|      |      |              |                  |   |   | a6 |      |
|      |      |              |                  |   |   | 7c |      |
|      |      |              |                  |   |   | 9a |      |
|      |      |              |                  |   |   | 31 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C3 |      |
|      |      |              |                  |   |   | 3- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C5 |      |
|      |      |              |                  |   |   | 2) |      |
|      |      |              |                  |   |   |    |      |
|      |      |              |                  |   |   | [[ |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 93 |      |
|      |      |              |                  |   |   | ]{ |      |
|      |      |              |                  |   |   | .u |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | 6c |      |
|      |      |              |                  |   |   | 5a |      |
|      |      |              |                  |   |   | d3 |      |
|      |      |              |                  |   |   | a7 |      |
|      |      |              |                  |   |   | 7b |      |
|      |      |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The          | Given that the   |   |   | [  |      |
|      |      | verification | verification key |   |   | [L |      |
|      |      | key text     | is saved on a    |   |   | 96 |      |
|      |      | envelope     | text envelope    |   |   | 6] |      |
|      |      | has:         | format, the type |   |   | {. |      |
|      |      |              | and description  |   |   | un |      |
|      |      | Type\        | fields are:      |   |   | de |      |
|      |      | \"CCons      |                  |   |   | rl |      |
|      |      | titutionalCo | Type\            |   |   | in |      |
|      |      | mmitteeColdV | \"CCons          |   |   | e} |      |
|      |      | erificationK | titutionalCommit |   |   | ]( |      |
|      |      | ey_ed25519\" | teeColdVerificat |   |   | ht |      |
|      |      |              | ionKey_ed25519\" |   |   | tp |      |
|      |      | Description\ |                  |   |   | s: |      |
|      |      | \"Co         | Description\     |   |   | // |      |
|      |      | nstitutional | \"Constitutional |   |   | gi |      |
|      |      | Committee    | Committee Cold   |   |   | th |      |
|      |      | Cold         | Verification     |   |   | ub |      |
|      |      | Verification | Key\"            |   |   | .c |      |
|      |      | Key\"        |                  |   |   | om |      |
|      |      |              |                  |   |   | /c |      |
|      |      |              |                  |   |   | ar |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | no |      |
|      |      |              |                  |   |   | -f |      |
|      |      |              |                  |   |   | ou |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | at |      |
|      |      |              |                  |   |   | io |      |
|      |      |              |                  |   |   | n/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | Ps |      |
|      |      |              |                  |   |   | /b |      |
|      |      |              |                  |   |   | lo |      |
|      |      |              |                  |   |   | b/ |      |
|      |      |              |                  |   |   | d6 |      |
|      |      |              |                  |   |   | c5 |      |
|      |      |              |                  |   |   | ad |      |
|      |      |              |                  |   |   | 3a |      |
|      |      |              |                  |   |   | 77 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 68 |      |
|      |      |              |                  |   |   | 4b |      |
|      |      |              |                  |   |   | c1 |      |
|      |      |              |                  |   |   | 9f |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | af |      |
|      |      |              |                  |   |   | b7 |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | 86 |      |
|      |      |              |                  |   |   | a6 |      |
|      |      |              |                  |   |   | 7c |      |
|      |      |              |                  |   |   | 9a |      |
|      |      |              |                  |   |   | 31 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C3 |      |
|      |      |              |                  |   |   | 3- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C5 |      |
|      |      |              |                  |   |   | 2) |      |
|      |      |              |                  |   |   |    |      |
|      |      |              |                  |   |   | [[ |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 93 |      |
|      |      |              |                  |   |   | ]{ |      |
|      |      |              |                  |   |   | .u |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | 6c |      |
|      |      |              |                  |   |   | 5a |      |
|      |      |              |                  |   |   | d3 |      |
|      |      |              |                  |   |   | a7 |      |
|      |      |              |                  |   |   | 7b |      |
|      |      |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Failing to   | Given the user   |   |   | [  |      |
|      |      | provide a    | has not inputted |   |   | [L |      |
|      |      | file name    | either           |   |   | 96 |      |
|      |      | for any of   | \--verif         |   |   | 6] |      |
|      |      | the flags    | ication-key-file |   |   | {. |      |
|      |      |              | OR               |   |   | un |      |
|      |      | \--verificat |                  |   |   | de |      |
|      |      | ion-key-file | \--              |   |   | rl |      |
|      |      |              | signing-key-file |   |   | in |      |
|      |      | \--sign      | parameters THEN  |   |   | e} |      |
|      |      | ing-key-file | the command      |   |   | ]( |      |
|      |      |              | fails and        |   |   | ht |      |
|      |      | fails with   | returns an error |   |   | tp |      |
|      |      | an           | to the users     |   |   | s: |      |
|      |      | appropriate  | informing them   |   |   | // |      |
|      |      | error        | to fill those    |   |   | gi |      |
|      |      | message.     | parameters in.   |   |   | th |      |
|      |      |              | The error        |   |   | ub |      |
|      |      |              | message should   |   |   | .c |      |
|      |      |              | prompt the user  |   |   | om |      |
|      |      |              | to consult the   |   |   | /c |      |
|      |      |              | command usage    |   |   | ar |      |
|      |      |              | (\--help)        |   |   | da |      |
|      |      |              |                  |   |   | no |      |
|      |      |              |                  |   |   | -f |      |
|      |      |              |                  |   |   | ou |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | at |      |
|      |      |              |                  |   |   | io |      |
|      |      |              |                  |   |   | n/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | Ps |      |
|      |      |              |                  |   |   | /b |      |
|      |      |              |                  |   |   | lo |      |
|      |      |              |                  |   |   | b/ |      |
|      |      |              |                  |   |   | d6 |      |
|      |      |              |                  |   |   | c5 |      |
|      |      |              |                  |   |   | ad |      |
|      |      |              |                  |   |   | 3a |      |
|      |      |              |                  |   |   | 77 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 68 |      |
|      |      |              |                  |   |   | 4b |      |
|      |      |              |                  |   |   | c1 |      |
|      |      |              |                  |   |   | 9f |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | af |      |
|      |      |              |                  |   |   | b7 |      |
|      |      |              |                  |   |   | 5b |      |
|      |      |              |                  |   |   | 48 |      |
|      |      |              |                  |   |   | 86 |      |
|      |      |              |                  |   |   | a6 |      |
|      |      |              |                  |   |   | 7c |      |
|      |      |              |                  |   |   | 9a |      |
|      |      |              |                  |   |   | 31 |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | -1 |      |
|      |      |              |                  |   |   | 69 |      |
|      |      |              |                  |   |   | 4/ |      |
|      |      |              |                  |   |   | RE |      |
|      |      |              |                  |   |   | AD |      |
|      |      |              |                  |   |   | ME |      |
|      |      |              |                  |   |   | .m |      |
|      |      |              |                  |   |   | d? |      |
|      |      |              |                  |   |   | pl |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | n= |      |
|      |      |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C3 |      |
|      |      |              |                  |   |   | 3- |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 66 |      |
|      |      |              |                  |   |   | C5 |      |
|      |      |              |                  |   |   | 2) |      |
|      |      |              |                  |   |   |    |      |
|      |      |              |                  |   |   | [[ |      |
|      |      |              |                  |   |   | L9 |      |
|      |      |              |                  |   |   | 93 |      |
|      |      |              |                  |   |   | ]{ |      |
|      |      |              |                  |   |   | .u |      |
|      |      |              |                  |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /d |      |
|      |      |              |                  |   |   | 6c |      |
|      |      |              |                  |   |   | 5a |      |
|      |      |              |                  |   |   | d3 |      |
|      |      |              |                  |   |   | a7 |      |
|      |      |              |                  |   |   | 7b |      |
|      |      |              |                  |   |   | 46 |      |
|      |      |              |                  |   |   | 84 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | 19 |      |
|      |      |              |                  |   |   | f3 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | 75 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | 88 |      |
|      |      |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 67 |      |
|      |      |              |                  |   |   | c9 |      |
|      |      |              |                  |   |   | a3 |      |
|      |      |              |                  |   |   | 1/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As a | [The feature | Typing           |   |   | [[ |      |
| LI05 | c    | im           | [cardano-cli     |   |   | L9 |      |
|      | ommi | plementation | conway           |   |   | 93 |      |
|      | ttee | should       | governance       |   |   | ]{ |      |
|      | me   | include a    | committee        |   |   | .u |      |
|      | mber | new command  | create-h         |   |   | nd |      |
|      |      | in the       | ot-key-authoriza |   |   | er |      |
|      | I    | cardano-     | tion-certificate |   |   | li |      |
|      | want | cli:]{.mark} | with accepted    |   |   | ne |      |
|      | to   |              | input parameters |   |   | }] |      |
|      | i    | [cardano-cli | generates a hot  |   |   | (h |      |
|      | ssue | conway       | key              |   |   | tt |      |
|      | a    | governance   | authorization    |   |   | ps |      |
|      | a    | committee    | certificate. If  |   |   | :/ |      |
|      | utho | create-hot-k | a parameter or   |   |   | /g |      |
|      | riza | ey-authoriza | the command      |   |   | it |      |
|      | tion | tion-certifi | format is        |   |   | hu |      |
|      | cer  | cate]{.mark} | incorrect an     |   |   | b. |      |
|      | tifi |              | error is         |   |   | co |      |
|      | cate |              | raised]{.mark}   |   |   | m/ |      |
|      | from |              |                  |   |   | ca |      |
|      | my   |              |                  |   |   | rd |      |
|      | cold |              |                  |   |   | an |      |
|      | key  |              |                  |   |   | o- |      |
|      | to a |              |                  |   |   | fo |      |
|      | hot  |              |                  |   |   | un |      |
|      | key  |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      | So   |              |                  |   |   | on |      |
|      | that |              |                  |   |   | /C |      |
|      | I    |              |                  |   |   | IP |      |
|      | can  |              |                  |   |   | s/ |      |
|      | sign |              |                  |   |   | bl |      |
|      | my   |              |                  |   |   | ob |      |
|      | v    |              |                  |   |   | /0 |      |
|      | otes |              |                  |   |   | f6 |      |
|      | u    |              |                  |   |   | 4c |      |
|      | sing |              |                  |   |   | 52 |      |
|      | the  |              |                  |   |   | fe |      |
|      | hot  |              |                  |   |   | 13 |      |
|      | key  |              |                  |   |   | 50 |      |
|      | and  |              |                  |   |   | b4 |      |
|      | keep |              |                  |   |   | e9 |      |
|      | the  |              |                  |   |   | 3c |      |
|      | cold |              |                  |   |   | 23 |      |
|      | key  |              |                  |   |   | f6 |      |
|      | in   |              |                  |   |   | bc |      |
|      | cold |              |                  |   |   | ed |      |
|      | sto  |              |                  |   |   | 92 |      |
|      | rage |              |                  |   |   | d4 |      |
|      | and  |              |                  |   |   | ca |      |
|      | can  |              |                  |   |   | 57 |      |
|      | a    |              |                  |   |   | 65 |      |
|      | utho |              |                  |   |   | 38 |      |
|      | rise |              |                  |   |   | e/ |      |
|      | a    |              |                  |   |   | CI |      |
|      | new  |              |                  |   |   | P- |      |
|      | hot  |              |                  |   |   | 16 |      |
|      | key  |              |                  |   |   | 94 |      |
|      | in   |              |                  |   |   | /R |      |
|      | case |              |                  |   |   | EA |      |
|      | the  |              |                  |   |   | DM |      |
|      | orig |              |                  |   |   | E. |      |
|      | inal |              |                  |   |   | md |      |
|      | one  |              |                  |   |   | ?p |      |
|      | is   |              |                  |   |   | la |      |
|      | comp |              |                  |   |   | in |      |
|      | romi |              |                  |   |   | =1 |      |
|      | sed. |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The command  | The command      |   |   | [[ |      |
|      |      | should       | allows passing   |   |   | L9 |      |
|      |      | accept the   | credentials as   |   |   | 93 |      |
|      |      | necessary    | follows          |   |   | ]{ |      |
|      |      | flags:       |                  |   |   | .u |      |
|      |      |              | Cold             |   |   | nd |      |
|      |      | \            | verification key |   |   | er |      |
|      |      | --cold-verif | \<- string       |   |   | li |      |
|      |      | ication-key, |                  |   |   | ne |      |
|      |      | \--col       | Cold             |   |   | }] |      |
|      |      | d-verificati | verification key |   |   | (h |      |
|      |      | on-key-file, | file \<- file    |   |   | tt |      |
|      |      | \--col       |                  |   |   | ps |      |
|      |      | d-verificati | Cold             |   |   | :/ |      |
|      |      | on-key-hash, | verification key |   |   | /g |      |
|      |      | \--hot-verif | hash \<- string  |   |   | it |      |
|      |      | ication-key, |                  |   |   | hu |      |
|      |      | \--ho        | Hot verification |   |   | b. |      |
|      |      | t-verificati | key \<- string   |   |   | co |      |
|      |      | on-key-file, |                  |   |   | m/ |      |
|      |      | \--ho        | Hot verification |   |   | ca |      |
|      |      | t-verificati | key file \<-     |   |   | rd |      |
|      |      | on-key-hash, | file             |   |   | an |      |
|      |      | and          |                  |   |   | o- |      |
|      |      | \--out-file. | Hot verification |   |   | fo |      |
|      |      |              | key hash \<-     |   |   | un |      |
|      |      |              | string\          |   |   | da |      |
|      |      |              | \                |   |   | ti |      |
|      |      |              | Failing to       |   |   | on |      |
|      |      |              | provide the      |   |   | /C |      |
|      |      |              | right input      |   |   | IP |      |
|      |      |              | results in a     |   |   | s/ |      |
|      |      |              | clear error      |   |   | bl |      |
|      |      |              | message that     |   |   | ob |      |
|      |      |              | helps the user   |   |   | /0 |      |
|      |      |              | to identify the  |   |   | f6 |      |
|      |      |              | problem          |   |   | 4c |      |
|      |      |              |                  |   |   | 52 |      |
|      |      |              |                  |   |   | fe |      |
|      |      |              |                  |   |   | 13 |      |
|      |      |              |                  |   |   | 50 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | e9 |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | 23 |      |
|      |      |              |                  |   |   | f6 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | ed |      |
|      |      |              |                  |   |   | 92 |      |
|      |      |              |                  |   |   | d4 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | 57 |      |
|      |      |              |                  |   |   | 65 |      |
|      |      |              |                  |   |   | 38 |      |
|      |      |              |                  |   |   | e/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Running the | Given that the   |   |   | [[ |      |
|      |      | command with | user specifies a |   |   | L9 |      |
|      |      | the          | valid path and   |   |   | 93 |      |
|      |      | appropriate  | file name, then  |   |   | ]{ |      |
|      |      | flags should | the command      |   |   | .u |      |
|      |      | generate a   | produces a Cold  |   |   | nd |      |
|      |      | hot key      | to Hot           |   |   | er |      |
|      |      | a            | authorization    |   |   | li |      |
|      |      | uthorization | certificate on   |   |   | ne |      |
|      |      | certificate  | the right        |   |   | }] |      |
|      |      | and be saved | location and     |   |   | (h |      |
|      |      | in the       | name.            |   |   | tt |      |
|      |      | specified    |                  |   |   | ps |      |
|      |      | output       |                  |   |   | :/ |      |
|      |      | f            |                  |   |   | /g |      |
|      |      | ile.]{.mark} |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /0 |      |
|      |      |              |                  |   |   | f6 |      |
|      |      |              |                  |   |   | 4c |      |
|      |      |              |                  |   |   | 52 |      |
|      |      |              |                  |   |   | fe |      |
|      |      |              |                  |   |   | 13 |      |
|      |      |              |                  |   |   | 50 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | e9 |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | 23 |      |
|      |      |              |                  |   |   | f6 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | ed |      |
|      |      |              |                  |   |   | 92 |      |
|      |      |              |                  |   |   | d4 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | 57 |      |
|      |      |              |                  |   |   | 65 |      |
|      |      |              |                  |   |   | 38 |      |
|      |      |              |                  |   |   | e/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The hot key | Given that the   |   |   | [[ |      |
|      |      | a            | authorization    |   |   | L9 |      |
|      |      | uthorization | certificate is   |   |   | 93 |      |
|      |      | certificate  | saved, then it   |   |   | ]{ |      |
|      |      | should       | is in a text     |   |   | .u |      |
|      |      | follow the   | envelope format  |   |   | nd |      |
|      |      | text         | consisting of a  |   |   | er |      |
|      |      | envelope     | json object with |   |   | li |      |
|      |      | format of    | type,            |   |   | ne |      |
|      |      | other        | description and  |   |   | }] |      |
|      |      | existing     | cbor hex fields. |   |   | (h |      |
|      |      | c            |                  |   |   | tt |      |
|      |      | ertificates, |                  |   |   | ps |      |
|      |      | including    |                  |   |   | :/ |      |
|      |      | the type,    |                  |   |   | /g |      |
|      |      | description, |                  |   |   | it |      |
|      |      | and CBOR hex |                  |   |   | hu |      |
|      |      | va           |                  |   |   | b. |      |
|      |      | lue.]{.mark} |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      | [{]{.mark}   |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      | [\"type\":   |                  |   |   | an |      |
|      |      | \"Cert       |                  |   |   | o- |      |
|      |      | ificateConwa |                  |   |   | fo |      |
|      |      | y\",]{.mark} |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      | [\"de        |                  |   |   | ti |      |
|      |      | scription\": |                  |   |   | on |      |
|      |      | \"Co         |                  |   |   | /C |      |
|      |      | nstitutional |                  |   |   | IP |      |
|      |      | Committee    |                  |   |   | s/ |      |
|      |      | Hot Key      |                  |   |   | bl |      |
|      |      | A            |                  |   |   | ob |      |
|      |      | uthorization |                  |   |   | /0 |      |
|      |      | Certificat   |                  |   |   | f6 |      |
|      |      | e\",]{.mark} |                  |   |   | 4c |      |
|      |      |              |                  |   |   | 52 |      |
|      |      | [            |                  |   |   | fe |      |
|      |      | \"cborHex\": |                  |   |   | 13 |      |
|      |      | \"\"]{.mark} |                  |   |   | 50 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      | [}]{.mark}   |                  |   |   | e9 |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | 23 |      |
|      |      |              |                  |   |   | f6 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | ed |      |
|      |      |              |                  |   |   | 92 |      |
|      |      |              |                  |   |   | d4 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | 57 |      |
|      |      |              |                  |   |   | 65 |      |
|      |      |              |                  |   |   | 38 |      |
|      |      |              |                  |   |   | e/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The type of  | The type field   |   |   | [[ |      |
|      |      | the          | ont the text     |   |   | L9 |      |
|      |      | certificate  | envelope of the  |   |   | 93 |      |
|      |      | should be:   | certificate is\  |   |   | ]{ |      |
|      |      | \"Certifi    | \"Cer            |   |   | .u |      |
|      |      | cateConway\" | tificateConway\" |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }] |      |
|      |      |              |                  |   |   | (h |      |
|      |      |              |                  |   |   | tt |      |
|      |      |              |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /0 |      |
|      |      |              |                  |   |   | f6 |      |
|      |      |              |                  |   |   | 4c |      |
|      |      |              |                  |   |   | 52 |      |
|      |      |              |                  |   |   | fe |      |
|      |      |              |                  |   |   | 13 |      |
|      |      |              |                  |   |   | 50 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | e9 |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | 23 |      |
|      |      |              |                  |   |   | f6 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | ed |      |
|      |      |              |                  |   |   | 92 |      |
|      |      |              |                  |   |   | d4 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | 57 |      |
|      |      |              |                  |   |   | 65 |      |
|      |      |              |                  |   |   | 38 |      |
|      |      |              |                  |   |   | e/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | The description  |   |   | [[ |      |
|      |      | description  | field on the     |   |   | L9 |      |
|      |      | of the       | text envelope of |   |   | 93 |      |
|      |      | certificate  | the certificate  |   |   | ]{ |      |
|      |      | should       | is\              |   |   | .u |      |
|      |      | be:]{.mark}  | [\"Committee     |   |   | nd |      |
|      |      |              | HotKey           |   |   | er |      |
|      |      | [\"Committee | Authorization    |   |   | li |      |
|      |      | HotKey       | Certi            |   |   | ne |      |
|      |      | A            | ficate\"]{.mark} |   |   | }] |      |
|      |      | uthorization |                  |   |   | (h |      |
|      |      | Certifica    |                  |   |   | tt |      |
|      |      | te\"]{.mark} |                  |   |   | ps |      |
|      |      |              |                  |   |   | :/ |      |
|      |      |              |                  |   |   | /g |      |
|      |      |              |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /0 |      |
|      |      |              |                  |   |   | f6 |      |
|      |      |              |                  |   |   | 4c |      |
|      |      |              |                  |   |   | 52 |      |
|      |      |              |                  |   |   | fe |      |
|      |      |              |                  |   |   | 13 |      |
|      |      |              |                  |   |   | 50 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | e9 |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | 23 |      |
|      |      |              |                  |   |   | f6 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | ed |      |
|      |      |              |                  |   |   | 92 |      |
|      |      |              |                  |   |   | d4 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | 57 |      |
|      |      |              |                  |   |   | 65 |      |
|      |      |              |                  |   |   | 38 |      |
|      |      |              |                  |   |   | e/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Given that the   |   |   | [[ |      |
|      |      | certificate  | authorization    |   |   | L9 |      |
|      |      | must comply  | certificate is   |   |   | 93 |      |
|      |      | with the     | saved,then it is |   |   | ]{ |      |
|      |      | c            | on the form of a |   |   | .u |      |
|      |      | ddl:]{.mark} | text envelope    |   |   | nd |      |
|      |      |              | consisting of a  |   |   | er |      |
|      |      | [auth_commit | json object with |   |   | li |      |
|      |      | tee_hot_cert | type,            |   |   | ne |      |
|      |      | = (14,       | description and  |   |   | }] |      |
|      |      | co           | cbor hex fields  |   |   | (h |      |
|      |      | mmittee_cold | , where          |   |   | tt |      |
|      |      | _credential, |                  |   |   | ps |      |
|      |      | committee    | Cbor hex         |   |   | :/ |      |
|      |      | _hot_credent | conforms to the  |   |   | /g |      |
|      |      | ial)]{.mark} | authorization    |   |   | it |      |
|      |      |              | certificate as   |   |   | hu |      |
|      |      |              | defined on the   |   |   | b. |      |
|      |      |              | cddl             |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              | [auth_co         |   |   | ca |      |
|      |      |              | mmittee_hot_cert |   |   | rd |      |
|      |      |              | = (14,           |   |   | an |      |
|      |      |              | committee_       |   |   | o- |      |
|      |      |              | cold_credential, |   |   | fo |      |
|      |      |              | c                |   |   | un |      |
|      |      |              | ommittee_hot_cre |   |   | da |      |
|      |      |              | dential)]{.mark} |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /0 |      |
|      |      |              |                  |   |   | f6 |      |
|      |      |              |                  |   |   | 4c |      |
|      |      |              |                  |   |   | 52 |      |
|      |      |              |                  |   |   | fe |      |
|      |      |              |                  |   |   | 13 |      |
|      |      |              |                  |   |   | 50 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | e9 |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | 23 |      |
|      |      |              |                  |   |   | f6 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | ed |      |
|      |      |              |                  |   |   | 92 |      |
|      |      |              |                  |   |   | d4 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | 57 |      |
|      |      |              |                  |   |   | 65 |      |
|      |      |              |                  |   |   | 38 |      |
|      |      |              |                  |   |   | e/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The command  | The command      |   |   | [[ |      |
|      |      | should       | should handle    |   |   | L9 |      |
|      |      | handle       | potential        |   |   | 93 |      |
|      |      | potential    | errors, such as  |   |   | ]{ |      |
|      |      | errors, such | missing or       |   |   | .u |      |
|      |      | as missing   | invalid flags,   |   |   | nd |      |
|      |      | or invalid   | and provide      |   |   | er |      |
|      |      | flags, and   | appropriate      |   |   | li |      |
|      |      | provide      | error messages   |   |   | ne |      |
|      |      | appropriate  | indicating the   |   |   | }] |      |
|      |      | error        | missing or       |   |   | (h |      |
|      |      | messages     | required         |   |   | tt |      |
|      |      | indicating   | parameters.      |   |   | ps |      |
|      |      | the missing  |                  |   |   | :/ |      |
|      |      | or required  |                  |   |   | /g |      |
|      |      | parameters.  |                  |   |   | it |      |
|      |      |              |                  |   |   | hu |      |
|      |      |              |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /0 |      |
|      |      |              |                  |   |   | f6 |      |
|      |      |              |                  |   |   | 4c |      |
|      |      |              |                  |   |   | 52 |      |
|      |      |              |                  |   |   | fe |      |
|      |      |              |                  |   |   | 13 |      |
|      |      |              |                  |   |   | 50 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | e9 |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | 23 |      |
|      |      |              |                  |   |   | f6 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | ed |      |
|      |      |              |                  |   |   | 92 |      |
|      |      |              |                  |   |   | d4 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | 57 |      |
|      |      |              |                  |   |   | 65 |      |
|      |      |              |                  |   |   | 38 |      |
|      |      |              |                  |   |   | e/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | D            | Typing           |   |   | [[ |      |
|      |      | ocumentation | [cardano-cli     |   |   | L9 |      |
|      |      | should be    | conway           |   |   | 93 |      |
|      |      | provided,    | governance       |   |   | ]{ |      |
|      |      | including a  | committee        |   |   | .u |      |
|      |      | c            | create-h         |   |   | nd |      |
|      |      | orresponding | ot-key-authoriza |   |   | er |      |
|      |      | CLI usage,   | tion-certificate |   |   | li |      |
|      |      | describing   | ----help         |   |   | ne |      |
|      |      | the feature, | displays command |   |   | }] |      |
|      |      | its purpose, | usage]{.mark}    |   |   | (h |      |
|      |      | and how to   |                  |   |   | tt |      |
|      |      | use it,      |                  |   |   | ps |      |
|      |      | along with   |                  |   |   | :/ |      |
|      |      | the expected |                  |   |   | /g |      |
|      |      | types of     |                  |   |   | it |      |
|      |      | inputs and   |                  |   |   | hu |      |
|      |      | outputs.     |                  |   |   | b. |      |
|      |      |              |                  |   |   | co |      |
|      |      |              |                  |   |   | m/ |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | rd |      |
|      |      |              |                  |   |   | an |      |
|      |      |              |                  |   |   | o- |      |
|      |      |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      |      |              |                  |   |   | da |      |
|      |      |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      |      |              |                  |   |   | IP |      |
|      |      |              |                  |   |   | s/ |      |
|      |      |              |                  |   |   | bl |      |
|      |      |              |                  |   |   | ob |      |
|      |      |              |                  |   |   | /0 |      |
|      |      |              |                  |   |   | f6 |      |
|      |      |              |                  |   |   | 4c |      |
|      |      |              |                  |   |   | 52 |      |
|      |      |              |                  |   |   | fe |      |
|      |      |              |                  |   |   | 13 |      |
|      |      |              |                  |   |   | 50 |      |
|      |      |              |                  |   |   | b4 |      |
|      |      |              |                  |   |   | e9 |      |
|      |      |              |                  |   |   | 3c |      |
|      |      |              |                  |   |   | 23 |      |
|      |      |              |                  |   |   | f6 |      |
|      |      |              |                  |   |   | bc |      |
|      |      |              |                  |   |   | ed |      |
|      |      |              |                  |   |   | 92 |      |
|      |      |              |                  |   |   | d4 |      |
|      |      |              |                  |   |   | ca |      |
|      |      |              |                  |   |   | 57 |      |
|      |      |              |                  |   |   | 65 |      |
|      |      |              |                  |   |   | 38 |      |
|      |      |              |                  |   |   | e/ |      |
|      |      |              |                  |   |   | CI |      |
|      |      |              |                  |   |   | P- |      |
|      |      |              |                  |   |   | 16 |      |
|      |      |              |                  |   |   | 94 |      |
|      |      |              |                  |   |   | /R |      |
|      |      |              |                  |   |   | EA |      |
|      |      |              |                  |   |   | DM |      |
|      |      |              |                  |   |   | E. |      |
|      |      |              |                  |   |   | md |      |
|      |      |              |                  |   |   | ?p |      |
|      |      |              |                  |   |   | la |      |
|      |      |              |                  |   |   | in |      |
|      |      |              |                  |   |   | =1 |      |
|      |      |              |                  |   |   | #L |      |
|      |      |              |                  |   |   | 99 |      |
|      |      |              |                  |   |   | 3) |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As a | [The command | Typing           |   |   |    |      |
| LI06 | p    | generates    | [cardano-cli     |   |   |    |      |
|      | oten | the blake2b  | conway           |   |   |    |      |
|      | tial | 256 hash of  | governance       |   |   |    |      |
|      | co   | the          | committee        |   |   |    |      |
|      | nsti | verification | key-hash with    |   |   |    |      |
|      | tuti | key]{.mark}  | accepted input   |   |   |    |      |
|      | onal |              | parameters       |   |   |    |      |
|      | c    | [cardano-cli | generates        |   |   |    |      |
|      | ommi | conway       | blake2b 256 hash |   |   |    |      |
|      | ttee | governance   | of the           |   |   |    |      |
|      | me   | committee    | verification     |   |   |    |      |
|      | mber | key-         | key. If a        |   |   |    |      |
|      |      | hash]{.mark} | parameter or the |   |   |    |      |
|      | I    |              | command format   |   |   |    |      |
|      | want |              | is incorrect an  |   |   |    |      |
|      | to   |              | error is         |   |   |    |      |
|      | gene |              | raised]{.mark}   |   |   |    |      |
|      | rate |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | key  |              |                  |   |   |    |      |
|      | ha   |              |                  |   |   |    |      |
|      | shes |              |                  |   |   |    |      |
|      | for  |              |                  |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | cold |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | hot  |              |                  |   |   |    |      |
|      | keys |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | they |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | used |              |                  |   |   |    |      |
|      | by   |              |                  |   |   |    |      |
|      | t    |              |                  |   |   |    |      |
|      | hird |              |                  |   |   |    |      |
|      | par  |              |                  |   |   |    |      |
|      | ties |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | pro  |              |                  |   |   |    |      |
|      | pose |              |                  |   |   |    |      |
|      | me   |              |                  |   |   |    |      |
|      | as a |              |                  |   |   |    |      |
|      | new  |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | ommi |              |                  |   |   |    |      |
|      | ttee |              |                  |   |   |    |      |
|      | me   |              |                  |   |   |    |      |
|      | mber |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | for  |              |                  |   |   |    |      |
|      | id   |              |                  |   |   |    |      |
|      | enti |              |                  |   |   |    |      |
|      | fica |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | purp |              |                  |   |   |    |      |
|      | oses |              |                  |   |   |    |      |
|      | once |              |                  |   |   |    |      |
|      | Ive  |              |                  |   |   |    |      |
|      | been |              |                  |   |   |    |      |
|      | ele  |              |                  |   |   |    |      |
|      | cted |              |                  |   |   |    |      |
|      | as   |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | ommi |              |                  |   |   |    |      |
|      | ttee |              |                  |   |   |    |      |
|      | me   |              |                  |   |   |    |      |
|      | mber |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Accepts the  | Both flags are   |   |   |    |      |
|      |      | flags        | mandatory and    |   |   |    |      |
|      |      |              | each produces    |   |   |    |      |
|      |      | [\--         | the              |   |   |    |      |
|      |      | verification | corresponding    |   |   |    |      |
|      |      | -key]{.mark} | verification or  |   |   |    |      |
|      |      | [\--verif    | signing key file |   |   |    |      |
|      |      | ication-key- |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | To provide   |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | key.         |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Given that the   |   |   |    |      |
|      |      | gives the    | user specifies   |   |   |    |      |
|      |      | option       | the [--out-file  |   |   |    |      |
|      |      | --out-f      | parameter        |   |   |    |      |
|      |      | ile.]{.mark} | and]{.mark} a    |   |   |    |      |
|      |      | If the       | valid path and   |   |   |    |      |
|      |      | \--out-file  | file name, Then  |   |   |    |      |
|      |      | flag is      | the key hash is  |   |   |    |      |
|      |      | provided,    | saved on that    |   |   |    |      |
|      |      | the key hash | file and         |   |   |    |      |
|      |      | should be    | location.        |   |   |    |      |
|      |      | saved to the |                  |   |   |    |      |
|      |      | specified    |                  |   |   |    |      |
|      |      | file.        |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | If the       | Given that the   |   |   |    |      |
|      |      | \--out-file  | user has not     |   |   |    |      |
|      |      | flag is not  | specified the    |   |   |    |      |
|      |      | provided,    | [--out-file      |   |   |    |      |
|      |      | the key hash | parameter then   |   |   |    |      |
|      |      | should be    | the key hash     |   |   |    |      |
|      |      | printed to   | must returned in |   |   |    |      |
|      |      | the standard | clear text       |   |   |    |      |
|      |      | output       | through stdout   |   |   |    |      |
|      |      | (stdout) in  | (cmd             |   |   |    |      |
|      |      | a readable   | output)]{.mark}  |   |   |    |      |
|      |      | format.      |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The command  | Given that the   |   |   |    |      |
|      |      | should       | user has         |   |   |    |      |
|      |      | handle       | executed the     |   |   |    |      |
|      |      | potential    | correct command  |   |   |    |      |
|      |      | errors, such | but has either   |   |   |    |      |
|      |      | as missing   | filled           |   |   |    |      |
|      |      | flags or     | incorrectly any  |   |   |    |      |
|      |      | invalid      | of the           |   |   |    |      |
|      |      | input, and   | parameters,      |   |   |    |      |
|      |      | provide      | missed any       |   |   |    |      |
|      |      | appropriate  | mandatory flag   |   |   |    |      |
|      |      | error        | and/or parameter |   |   |    |      |
|      |      | messages or  | then an          |   |   |    |      |
|      |      | exceptions   | exception should |   |   |    |      |
|      |      | to guide the | be raised and an |   |   |    |      |
|      |      | user.        | error message    |   |   |    |      |
|      |      |              | should be        |   |   |    |      |
|      |      |              | returned with    |   |   |    |      |
|      |      |              | clear indication |   |   |    |      |
|      |      |              | as to how to fix |   |   |    |      |
|      |      |              | the issue. When  |   |   |    |      |
|      |      |              | not feasible,    |   |   |    |      |
|      |      |              | the user should  |   |   |    |      |
|      |      |              | be directed to   |   |   |    |      |
|      |      |              | the usage page   |   |   |    |      |
|      |      |              | of the command   |   |   |    |      |
|      |      |              | ([cardano-cli    |   |   |    |      |
|      |      |              | conway           |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | committee        |   |   |    |      |
|      |      |              | key-hash]{.mark} |   |   |    |      |
|      |      |              | \--help)         |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | D            | Typing           |   |   |    |      |
|      |      | ocumentation | [cardano-cli     |   |   |    |      |
|      |      | should be    | conway           |   |   |    |      |
|      |      | provided,    | governance       |   |   |    |      |
|      |      | including a  | committee        |   |   |    |      |
|      |      | c            | key-hash]{.mark} |   |   |    |      |
|      |      | orresponding | \--help display  |   |   |    |      |
|      |      | CLI usage,   | the command      |   |   |    |      |
|      |      | describing   | usage page       |   |   |    |      |
|      |      | the feature, |                  |   |   |    |      |
|      |      | its purpose, |                  |   |   |    |      |
|      |      | and how to   |                  |   |   |    |      |
|      |      | use it,      |                  |   |   |    |      |
|      |      | along with   |                  |   |   |    |      |
|      |      | the expected |                  |   |   |    |      |
|      |      | types of     |                  |   |   |    |      |
|      |      | inputs and   |                  |   |   |    |      |
|      |      | outputs.     |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As a | The command  | Typing           |   |   |    |      |
| LI07 | co   | should be    | cardano-cli      |   |   |    |      |
|      | nsti | implemented  | governance       |   |   |    |      |
|      | tuti | in the       | committee        |   |   |    |      |
|      | onal | cardano-cli  | cre              |   |   |    |      |
|      | c    | as           | ate-cold-resigna |   |   |    |      |
|      | ommi | cardano-cli  | tion-certificate |   |   |    |      |
|      | ttee | governance   | with accepted    |   |   |    |      |
|      | me   | committee    | input parameters |   |   |    |      |
|      | mber | create-cold  | generates a cold |   |   |    |      |
|      |      | -resignation | resignation      |   |   |    |      |
|      | I    | -certificate | certificate.     |   |   |    |      |
|      | want |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | able |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | gene |              |                  |   |   |    |      |
|      | rate |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | res  |              |                  |   |   |    |      |
|      | igna |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | cer  |              |                  |   |   |    |      |
|      | tifi |              |                  |   |   |    |      |
|      | cate |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | i    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | su   |              |                  |   |   |    |      |
|      | bmit |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
|      | on a |              |                  |   |   |    |      |
|      | tra  |              |                  |   |   |    |      |
|      | nsac |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | si   |              |                  |   |   |    |      |
|      | gnal |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | ada  |              |                  |   |   |    |      |
|      | hol  |              |                  |   |   |    |      |
|      | ders |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I'm  |              |                  |   |   |    |      |
|      | r    |              |                  |   |   |    |      |
|      | esig |              |                  |   |   |    |      |
|      | ning |              |                  |   |   |    |      |
|      | from |              |                  |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | du   |              |                  |   |   |    |      |
|      | ties |              |                  |   |   |    |      |
|      | as   |              |                  |   |   |    |      |
|      | cc   |              |                  |   |   |    |      |
|      | me   |              |                  |   |   |    |      |
|      | mber |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The command  | The command      |   |   |    |      |
|      |      | should       | allows passing   |   |   |    |      |
|      |      | accept the   | credentials as   |   |   |    |      |
|      |      | following    | follows          |   |   |    |      |
|      |      | ways to      |                  |   |   |    |      |
|      |      | supply       | Cold             |   |   |    |      |
|      |      | credentials: | verification key |   |   |    |      |
|      |      | cold         | \<- string       |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | key file,    | Cold             |   |   |    |      |
|      |      | the cold     | verification key |   |   |    |      |
|      |      | verification | file \<- file    |   |   |    |      |
|      |      | key or the   |                  |   |   |    |      |
|      |      | cold         | Cold             |   |   |    |      |
|      |      | verification | verification key |   |   |    |      |
|      |      | key hash so  | hash \<- string  |   |   |    |      |
|      |      | it accepts   |                  |   |   |    |      |
|      |      | the          | If any of the    |   |   |    |      |
|      |      | following    | inputs has the   |   |   |    |      |
|      |      | flags:       | wrong format the |   |   |    |      |
|      |      |              | cli raises an    |   |   |    |      |
|      |      | \            | arrow message    |   |   |    |      |
|      |      | --cold-verif | indicating the   |   |   |    |      |
|      |      | ication-key, | missing or       |   |   |    |      |
|      |      |              | incorrect        |   |   |    |      |
|      |      | \--col       | parameter.       |   |   |    |      |
|      |      | d-verificati |                  |   |   |    |      |
|      |      | on-key-file, |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | \--col       |                  |   |   |    |      |
|      |      | d-verificati |                  |   |   |    |      |
|      |      | on-key-hash. |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The command  | The command      |   |   |    |      |
|      |      | allows an    | allows for an    |   |   |    |      |
|      |      | optional     | OPTIONAL anchor  |   |   |    |      |
|      |      | anchor       | comprised of a   |   |   |    |      |
|      |      | (url/hash)   | URL containing a |   |   |    |      |
|      |      | for the      | document where   |   |   |    |      |
|      |      | resigning\   | the resigning CC |   |   |    |      |
|      |      | cc member to | member expresses |   |   |    |      |
|      |      | express      | the motivations  |   |   |    |      |
|      |      | their\       | and the hash of  |   |   |    |      |
|      |      | motivation   | the document     |   |   |    |      |
|      |      | for          |                  |   |   |    |      |
|      |      | resigning.   | The CLI does not |   |   |    |      |
|      |      |              | check for the    |   |   |    |      |
|      |      |              | validity of the  |   |   |    |      |
|      |      |              | URL, the         |   |   |    |      |
|      |      |              | contents, or     |   |   |    |      |
|      |      |              | that the         |   |   |    |      |
|      |      |              | documents and    |   |   |    |      |
|      |      |              | declared hash    |   |   |    |      |
|      |      |              | match.           |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The          | Given that the   |   |   |    |      |
|      |      | resignation  | CC member        |   |   |    |      |
|      |      | certificate  | issuing the      |   |   |    |      |
|      |      | should be    | resignation      |   |   |    |      |
|      |      | saved in the | certificate      |   |   |    |      |
|      |      | specified    | provides a valid |   |   |    |      |
|      |      | output file  | path and file    |   |   |    |      |
|      |      | using the    | name, then the   |   |   |    |      |
|      |      | \--out-file  | certificate is   |   |   |    |      |
|      |      | flag.        | saved on the     |   |   |    |      |
|      |      |              | specified        |   |   |    |      |
|      |      |              | location.        |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The          | Given that the   |   |   |    |      |
|      |      | generated    | resignation      |   |   |    |      |
|      |      | resignation  | certificate is   |   |   |    |      |
|      |      | certificate  | saved, then it   |   |   |    |      |
|      |      | should be    | is in a text     |   |   |    |      |
|      |      | consistent   | envelope format  |   |   |    |      |
|      |      | with the     | consisting of a  |   |   |    |      |
|      |      | text         | json object with |   |   |    |      |
|      |      | envelope     | type,            |   |   |    |      |
|      |      | format of    | description and  |   |   |    |      |
|      |      | existing     | cbor hex fields. |   |   |    |      |
|      |      | certificates |                  |   |   |    |      |
|      |      | in Cardano,  |                  |   |   |    |      |
|      |      | including    |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | specified    |                  |   |   |    |      |
|      |      | JSON         |                  |   |   |    |      |
|      |      | structure    |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | correct      |                  |   |   |    |      |
|      |      | type,        |                  |   |   |    |      |
|      |      | description, |                  |   |   |    |      |
|      |      | and          |                  |   |   |    |      |
|      |      | CBOR-encoded |                  |   |   |    |      |
|      |      | value.       |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | {            |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | \"type\":    |                  |   |   |    |      |
|      |      | \"Certific   |                  |   |   |    |      |
|      |      | ateConway\", |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | \"de         |                  |   |   |    |      |
|      |      | scription\": |                  |   |   |    |      |
|      |      | \"Co         |                  |   |   |    |      |
|      |      | nstitutional |                  |   |   |    |      |
|      |      | Committee    |                  |   |   |    |      |
|      |      | Cold Key     |                  |   |   |    |      |
|      |      | Resignation  |                  |   |   |    |      |
|      |      | Ce           |                  |   |   |    |      |
|      |      | rtificate\", |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | \"cborHex\": |                  |   |   |    |      |
|      |      | \"\"         |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | }            |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The          | Given that the   |   |   |    |      |
|      |      | certificate  | certificate is   |   |   |    |      |
|      |      | type should  | in a text        |   |   |    |      |
|      |      | be           | envelope format, |   |   |    |      |
|      |      | Conw         | then its type    |   |   |    |      |
|      |      | ayResignComm | is\              |   |   |    |      |
|      |      | itteeColdKey | \                |   |   |    |      |
|      |      | to indicate  | Type:            |   |   |    |      |
|      |      | a            | ConwayResign     |   |   |    |      |
|      |      | resignation  | CommitteeColdKey |   |   |    |      |
|      |      | of the       |                  |   |   |    |      |
|      |      | Committee    |                  |   |   |    |      |
|      |      | Cold Key.    |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The          | Given that the   |   |   |    |      |
|      |      | certificate  | certificate is   |   |   |    |      |
|      |      | description  | in a text        |   |   |    |      |
|      |      | should be    | envelope format, |   |   |    |      |
|      |      |              | then its         |   |   |    |      |
|      |      | \"de         | description      |   |   |    |      |
|      |      | scription\": | field is\        |   |   |    |      |
|      |      | \"Co         | \                |   |   |    |      |
|      |      | nstitutional | \"description\": |   |   |    |      |
|      |      | Committee    | \"Constitutional |   |   |    |      |
|      |      | Cold Key     | Committee Cold   |   |   |    |      |
|      |      | Resignation  | Key Resignation  |   |   |    |      |
|      |      | C            | Certificate\"    |   |   |    |      |
|      |      | ertificate\" |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The command  | Given that the   |   |   |    |      |
|      |      | should       | certificate is   |   |   |    |      |
|      |      | generate a   | in a text        |   |   |    |      |
|      |      | resignation  | envelope format, |   |   |    |      |
|      |      | certificate  | then its cbor    |   |   |    |      |
|      |      | according to | hex field        |   |   |    |      |
|      |      | the conway   | conforms to the  |   |   |    |      |
|      |      | cddl:        | conway cddl      |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | re           | resign_com       |   |   |    |      |
|      |      | sign_committ | mittee_cold_cert |   |   |    |      |
|      |      | ee_cold_cert | = (15,           |   |   |    |      |
|      |      | = (15,       | committee_       |   |   |    |      |
|      |      | co           | cold_credential, |   |   |    |      |
|      |      | mmittee_cold | anchor / null)   |   |   |    |      |
|      |      | _credential, |                  |   |   |    |      |
|      |      | anchor /     |                  |   |   |    |      |
|      |      | null)        |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The command  | If any required  |   |   |    |      |
|      |      | should       | input parameter  |   |   |    |      |
|      |      | handle       | is missing or    |   |   |    |      |
|      |      | potential    | incorrect, the   |   |   |    |      |
|      |      | errors, such | command should   |   |   |    |      |
|      |      | as missing   | raise an error   |   |   |    |      |
|      |      | or invalid   | indicating the   |   |   |    |      |
|      |      | flags or     | missing or       |   |   |    |      |
|      |      | keys, and    | incorrect        |   |   |    |      |
|      |      | provide      | parameter.       |   |   |    |      |
|      |      | appropriate  |                  |   |   |    |      |
|      |      | error        |                  |   |   |    |      |
|      |      | messages     |                  |   |   |    |      |
|      |      | indicating   |                  |   |   |    |      |
|      |      | the missing  |                  |   |   |    |      |
|      |      | or required  |                  |   |   |    |      |
|      |      | parameters.  |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | D            | Given that the   |   |   |    |      |
|      |      | ocumentation | user has         |   |   |    |      |
|      |      | should be    | executed the     |   |   |    |      |
|      |      | provided,    | correct command  |   |   |    |      |
|      |      | including a  | but has either   |   |   |    |      |
|      |      | c            | filled           |   |   |    |      |
|      |      | orresponding | incorrectly any  |   |   |    |      |
|      |      | CLI usage,   | of the           |   |   |    |      |
|      |      | describing   | parameters,      |   |   |    |      |
|      |      | the feature, | missed any       |   |   |    |      |
|      |      | its purpose, | mandatory flag   |   |   |    |      |
|      |      | and how to   | and/or parameter |   |   |    |      |
|      |      | use it,      | then an          |   |   |    |      |
|      |      | along with   | exception should |   |   |    |      |
|      |      | the expected | be raised and an |   |   |    |      |
|      |      | types of     | error message    |   |   |    |      |
|      |      | inputs and   | should be        |   |   |    |      |
|      |      | outputs.     | returned with    |   |   |    |      |
|      |      |              | clear indication |   |   |    |      |
|      |      |              | as to how to fix |   |   |    |      |
|      |      |              | the issue. When  |   |   |    |      |
|      |      |              | not feasible,    |   |   |    |      |
|      |      |              | the user should  |   |   |    |      |
|      |      |              | be directed to   |   |   |    |      |
|      |      |              | the usage page   |   |   |    |      |
|      |      |              | of the command   |   |   |    |      |
|      |      |              | ([cardano-cli    |   |   |    |      |
|      |      |              | governance       |   |   |    |      |
|      |      |              | committee        |   |   |    |      |
|      |      |              | create-cold      |   |   |    |      |
|      |      |              | -resignation-cer |   |   |    |      |
|      |      |              | tificate]{.mark} |   |   |    |      |
|      |      |              | \--help)         |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | The command  | Typing           |   |   |    |      |
| LI08 | an   | is           | cardano-cli      |   |   |    |      |
|      | ada  | implemented  | conway           |   |   |    |      |
|      | ho   | as\          | governance drep  |   |   |    |      |
|      | lder | \            | key-gen with     |   |   |    |      |
|      |      | cardano-cli  | accepted input   |   |   |    |      |
|      | I    | conway       | parameters       |   |   |    |      |
|      | want | governance   | generates an     |   |   |    |      |
|      | to   | drep key-gen | Ed25519 key pair |   |   |    |      |
|      | gene |              |                  |   |   |    |      |
|      | rate |              |                  |   |   |    |      |
|      | Ed2  |              |                  |   |   |    |      |
|      | 5519 |              |                  |   |   |    |      |
|      | keys |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | regi |              |                  |   |   |    |      |
|      | ster |              |                  |   |   |    |      |
|      | as a |              |                  |   |   |    |      |
|      | DRep |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The command  | The flag         |   |   |    |      |
|      |      | supports the | \--verif         |   |   |    |      |
|      |      | \--verificat | ication-key-file |   |   |    |      |
|      |      | ion-key-file | is mandatory,    |   |   |    |      |
|      |      | FILE option  |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | generated    |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | key will be  |                  |   |   |    |      |
|      |      | saved.       |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The command  | The flag         |   |   |    |      |
|      |      | supports the | \--              |   |   |    |      |
|      |      | \--sign      | signing-key-file |   |   |    |      |
|      |      | ing-key-file | is mandatory,    |   |   |    |      |
|      |      | FILE option  |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | generated    |                  |   |   |    |      |
|      |      | signing key  |                  |   |   |    |      |
|      |      | will be      |                  |   |   |    |      |
|      |      | saved. File  |                  |   |   |    |      |
|      |      | is saved on  |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | specified    |                  |   |   |    |      |
|      |      | path         |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [When the    | Given that the   |   |   |    |      |
|      |      | command is   | user specifies   |   |   |    |      |
|      |      | executed, it | valid paths and  |   |   |    |      |
|      |      | generates    | file names then, |   |   |    |      |
|      |      | both the     | the              |   |   |    |      |
|      |      | verification | corresponding    |   |   |    |      |
|      |      | key and      | verification and |   |   |    |      |
|      |      | signing      | signing key      |   |   |    |      |
|      |      | key]{.mark}  | files are saved  |   |   |    |      |
|      |      | File is      | on the paths     |   |   |    |      |
|      |      | saved on the | specified by the |   |   |    |      |
|      |      | specified    | user.            |   |   |    |      |
|      |      | path         |                  |   |   |    |      |
|      |      |              | If the paths do  |   |   |    |      |
|      |      |              | not exist or are |   |   |    |      |
|      |      |              | inaccessible, an |   |   |    |      |
|      |      |              | error message is |   |   |    |      |
|      |      |              | raised.          |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | The key      | Given that the   |   |   |    |      |
|      |      | generation   | verification and |   |   |    |      |
|      |      | should       | signing key      |   |   |    |      |
|      |      | follow the   | files are saved, |   |   |    |      |
|      |      | current      | then they are in |   |   |    |      |
|      |      | design for   | a text envelope  |   |   |    |      |
|      |      | key          | format           |   |   |    |      |
|      |      | generation   | consisting of a  |   |   |    |      |
|      |      | and output   | json object with |   |   |    |      |
|      |      | in an        | type,            |   |   |    |      |
|      |      | envelope     | description and  |   |   |    |      |
|      |      | format.      | cbor hex fields, |   |   |    |      |
|      |      |              | where:           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | {                |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | \"type\":        |   |   |    |      |
|      |      |              | \"DRepVerificati |   |   |    |      |
|      |      |              | onKey_ed25519\", |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | \"description\": |   |   |    |      |
|      |      |              | \"Delegate       |   |   |    |      |
|      |      |              | Representative   |   |   |    |      |
|      |      |              | Verification     |   |   |    |      |
|      |      |              | Key\",           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | \"cborHex\":     |   |   |    |      |
|      |      |              | \"\"             |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | }                |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | {                |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | \"type\":        |   |   |    |      |
|      |      |              | \"DRepSigni      |   |   |    |      |
|      |      |              | ngKey_ed25519\", |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | \"description\": |   |   |    |      |
|      |      |              | \"Delegate       |   |   |    |      |
|      |      |              | Representative   |   |   |    |      |
|      |      |              | VSigning Key\",  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | \"cborHex\":     |   |   |    |      |
|      |      |              | \"\"             |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | }                |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As a | [The command | Typing           |   |   |    |      |
| LI09 | DRep | is           | cardano-cli      |   |   |    |      |
|      |      | implemented  | conway           |   |   |    |      |
|      | I    | as           | governance drep  |   |   |    |      |
|      | want | cardano-cli  | id               |   |   |    |      |
|      | to   | conway       |                  |   |   |    |      |
|      | gene | governance   | with accepted    |   |   |    |      |
|      | rate | drep         | input parameters |   |   |    |      |
|      | a    | id]{.mark}   | generates a DRep |   |   |    |      |
|      | Drep |              | ID, [the         |   |   |    |      |
|      | Id   | [and         | blake2b-224 hash |   |   |    |      |
|      |      | generates    | digest of the    |   |   |    |      |
|      | So   | the          | serialised DRep  |   |   |    |      |
|      | that | blake2b-224  | credential       |   |   |    |      |
|      | ada  | hash digest  | (verification    |   |   |    |      |
|      | ho   | of the       | key)]{.mark}     |   |   |    |      |
|      | lder | serialised   |                  |   |   |    |      |
|      | can  | DRep         |                  |   |   |    |      |
|      | use  | credential   |                  |   |   |    |      |
|      | it   | (            |                  |   |   |    |      |
|      | to   | verification |                  |   |   |    |      |
|      | dele | key)]{.mark} |                  |   |   |    |      |
|      | gate |              |                  |   |   |    |      |
|      | t    |              |                  |   |   |    |      |
|      | heir |              |                  |   |   |    |      |
|      | v    |              |                  |   |   |    |      |
|      | otes |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | me   |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | vo   |              |                  |   |   |    |      |
|      | ting |              |                  |   |   |    |      |
|      | re   |              |                  |   |   |    |      |
|      | cord |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | tra  |              |                  |   |   |    |      |
|      | cked |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Using one of the |   |   |    |      |
|      |      | accepts      | flags is         |   |   |    |      |
|      |      | supplying    | mandatory, the   |   |   |    |      |
|      |      | the          | flags are        |   |   |    |      |
|      |      | verification | mutually         |   |   |    |      |
|      |      | key with     | exclusive and    |   |   |    |      |
|      |      | ei           | take a string    |   |   |    |      |
|      |      | ther]{.mark} | and file         |   |   |    |      |
|      |      |              | respectively:    |   |   |    |      |
|      |      | [\           |                  |   |   |    |      |
|      |      | \--drep-     | [\--drep-        |   |   |    |      |
|      |      | verification | verification-key |   |   |    |      |
|      |      | -key]{.mark} | \<-              |   |   |    |      |
|      |      |              | string]{.mark}   |   |   |    |      |
|      |      | [--dr        |                  |   |   |    |      |
|      |      | ep-verificat | [--drep-verif    |   |   |    |      |
|      |      | ion-key-file | ication-key-file |   |   |    |      |
|      |      | opt          | \<- file]{.mark} |   |   |    |      |
|      |      | ions]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Given that the   |   |   |    |      |
|      |      | supports the | user wants to    |   |   |    |      |
|      |      | \--out-file  | save the DrepId  |   |   |    |      |
|      |      | FILE option  | to a file, and   |   |   |    |      |
|      |      | (optional)   | specifies a      |   |   |    |      |
|      |      | to enable    | valid path and   |   |   |    |      |
|      |      | users to     | file name, then, |   |   |    |      |
|      |      | save the     | using the        |   |   |    |      |
|      |      | generated    | --out-file flag  |   |   |    |      |
|      |      | DRep ID to   | saves the drep   |   |   |    |      |
|      |      | the          | id to a file on  |   |   |    |      |
|      |      | specified    | the specified    |   |   |    |      |
|      |      | f            | location.\       |   |   |    |      |
|      |      | ile.]{.mark} | \                |   |   |    |      |
|      |      |              | If the specified |   |   |    |      |
|      |      |              | path does not    |   |   |    |      |
|      |      |              | exist or is      |   |   |    |      |
|      |      |              | inaccessible the |   |   |    |      |
|      |      |              | cli returns an   |   |   |    |      |
|      |      |              | error message.\  |   |   |    |      |
|      |      |              | \                |   |   |    |      |
|      |      |              | If the           |   |   |    |      |
|      |      |              | --out-flag is    |   |   |    |      |
|      |      |              | not used the     |   |   |    |      |
|      |      |              | Drep ID is       |   |   |    |      |
|      |      |              | printed on       |   |   |    |      |
|      |      |              | stdout           |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Given that the   |   |   |    |      |
|      |      | should       | optional         |   |   |    |      |
|      |      | support the  | \--output-format |   |   |    |      |
|      |      | an option to | flag is used,    |   |   |    |      |
|      |      | specify the  | and "bech32" is  |   |   |    |      |
|      |      | output       | given as an      |   |   |    |      |
|      |      | format\      | argument, then   |   |   |    |      |
|      |      | ]{.mark}     | the DRep Id is   |   |   |    |      |
|      |      |              | printed in       |   |   |    |      |
|      |      | [Accepted    | bech32 format    |   |   |    |      |
|      |      | output       | with the "drep"  |   |   |    |      |
|      |      | formats are  | prefix.          |   |   |    |      |
|      |      | \"hex\" and  |                  |   |   |    |      |
|      |      | \"bech32\",  | Given that the   |   |   |    |      |
|      |      | where        | optional         |   |   |    |      |
|      |      | \"bech32\"   | \--output-format |   |   |    |      |
|      |      | is the       | flag is used,    |   |   |    |      |
|      |      | default      | and the hex is   |   |   |    |      |
|      |      | for          | given as an      |   |   |    |      |
|      |      | mat.]{.mark} | argument, then   |   |   |    |      |
|      |      |              | the DRep Id is   |   |   |    |      |
|      |      |              | printed in hex   |   |   |    |      |
|      |      |              | format           |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | [If the          |   |   |    |      |
|      |      |              | \--output-format |   |   |    |      |
|      |      |              | STRING option is |   |   |    |      |
|      |      |              | not specified,   |   |   |    |      |
|      |      |              | the DRep ID      |   |   |    |      |
|      |      |              | should be        |   |   |    |      |
|      |      |              | displayed in     |   |   |    |      |
|      |      |              | \"bech32\"       |   |   |    |      |
|      |      |              | format by        |   |   |    |      |
|      |      |              | default.]{.mark} |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | [If the          |   |   |    |      |
|      |      | supports an  | \--out-file FILE |   |   |    |      |
|      |      | optional     | option is        |   |   |    |      |
|      |      | --out-file   | specified, the   |   |   |    |      |
|      |      | to save the  | generated DRep   |   |   |    |      |
|      |      | Drep Id to a | ID should be     |   |   |    |      |
|      |      | file]{.mark} | saved to the     |   |   |    |      |
|      |      |              | specified file,  |   |   |    |      |
|      |      |              | otherwise it is  |   |   |    |      |
|      |      |              | printed on       |   |   |    |      |
|      |      |              | stdout]{.mark}   |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The feature | Typing           |   |   |    |      |
|      |      | is           | cardano-cli      |   |   |    |      |
|      |      | well         | conway           |   |   |    |      |
|      |      | -documented, | governance drep  |   |   |    |      |
|      |      | providing    | id \--help       |   |   |    |      |
|      |      | clear usage  |                  |   |   |    |      |
|      |      | instructions | displays the     |   |   |    |      |
|      |      | for the      | command usage    |   |   |    |      |
|      |      | cardano-cli  | page             |   |   |    |      |
|      |      | conway       |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | drep id      |                  |   |   |    |      |
|      |      | comm         |                  |   |   |    |      |
|      |      | and.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | If any required  |   |   |    |      |
|      |      | handles      | input parameter  |   |   |    |      |
|      |      | errors       | is missing or    |   |   |    |      |
|      |      | gracefully   | incorrect, the   |   |   |    |      |
|      |      | and provides | command should   |   |   |    |      |
|      |      | helpful      | raise an error   |   |   |    |      |
|      |      | error        | indicating the   |   |   |    |      |
|      |      | messages     | missing or       |   |   |    |      |
|      |      | when         | incorrect        |   |   |    |      |
|      |      | required     | parameter.       |   |   |    |      |
|      |      | options are  |                  |   |   |    |      |
|      |      | missing or   |                  |   |   |    |      |
|      |      | invalid      |                  |   |   |    |      |
|      |      | inputs are   |                  |   |   |    |      |
|      |      | provi        |                  |   |   |    |      |
|      |      | ded.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As a | [The command | Running          |   |   |    |      |
| LI10 | DRep | is           |                  |   |   |    |      |
|      |      | implemented  | [cardano-cli     |   |   |    |      |
|      | I    | as]{.mark}   | conway           |   |   |    |      |
|      | want |              | governance drep  |   |   |    |      |
|      | to   | [cardano-cli | registration-cer |   |   |    |      |
|      | gene | conway       | tificate]{.mark} |   |   |    |      |
|      | rate | governance   | with accepted    |   |   |    |      |
|      | a    | drep         | input parameters |   |   |    |      |
|      | Drep | registra     | generates a drep |   |   |    |      |
|      | regi | tion-certifi | registration     |   |   |    |      |
|      | stra | cate]{.mark} | certificate.     |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | cer  |              |                  |   |   |    |      |
|      | tifi |              |                  |   |   |    |      |
|      | cate |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | su   |              |                  |   |   |    |      |
|      | bmit |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | on a |              |                  |   |   |    |      |
|      | tra  |              |                  |   |   |    |      |
|      | nsac |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | ada  |              |                  |   |   |    |      |
|      | hol  |              |                  |   |   |    |      |
|      | ders |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | dele |              |                  |   |   |    |      |
|      | gate |              |                  |   |   |    |      |
|      | t    |              |                  |   |   |    |      |
|      | heir |              |                  |   |   |    |      |
|      | v    |              |                  |   |   |    |      |
|      | otes |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | me.  |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | The flag         |   |   |    |      |
|      |      | requires the | \--key           |   |   |    |      |
|      |      | user to      | -reg-deposit-amt |   |   |    |      |
|      |      | provide the  | is mandatory and |   |   |    |      |
|      |      | amount       | takes the        |   |   |    |      |
|      |      | required for | deposit amount   |   |   |    |      |
|      |      | drep key     | in lovelace as   |   |   |    |      |
|      |      | deposit to   | argument.        |   |   |    |      |
|      |      | comply with  |                  |   |   |    |      |
|      |      | the conway   |                  |   |   |    |      |
|      |      | cddl -\>     |                  |   |   |    |      |
|      |      | "reg_drep_c  |                  |   |   |    |      |
|      |      | ert"]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | The command      |   |   |    |      |
|      |      | allows the   | presents the     |   |   |    |      |
|      |      | user to      | options to pass  |   |   |    |      |
|      |      | provide the  | the Drep         |   |   |    |      |
|      |      | DRep         | credential:\     |   |   |    |      |
|      |      | credential   | \                |   |   |    |      |
|      |      | in the       | \--drep-         |   |   |    |      |
|      |      | following    | verification-key |   |   |    |      |
|      |      | w            | STRING           |   |   |    |      |
|      |      | ays:]{.mark} |                  |   |   |    |      |
|      |      |              | \--drep-verif    |   |   |    |      |
|      |      | Drep         | ication-key-file |   |   |    |      |
|      |      | verification | FILE             |   |   |    |      |
|      |      | key          |                  |   |   |    |      |
|      |      |              | \--drep-id       |   |   |    |      |
|      |      | Drep         | STRING           |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | key file     | Using one of     |   |   |    |      |
|      |      |              | these is         |   |   |    |      |
|      |      | Drep Id      | mandatory but    |   |   |    |      |
|      |      |              | are mutually     |   |   |    |      |
|      |      |              | exclusive.       |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | Failing to       |   |   |    |      |
|      |      |              | provide the      |   |   |    |      |
|      |      |              | right input      |   |   |    |      |
|      |      |              | results in a     |   |   |    |      |
|      |      |              | clear error      |   |   |    |      |
|      |      |              | message that     |   |   |    |      |
|      |      |              | helps the user   |   |   |    |      |
|      |      |              | to identify the  |   |   |    |      |
|      |      |              | problem          |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | [Given that the  |   |   |    |      |
|      |      | allows       | user wants to    |   |   |    |      |
|      |      | adding an    | include an       |   |   |    |      |
|      |      | optional     | anchor with the  |   |   |    |      |
|      |      | anchor       | Dreps metadata,  |   |   |    |      |
|      |      | (url/hash)   | then the command |   |   |    |      |
|      |      | to submit    | requires both    |   |   |    |      |
|      |      | any drep     | the url and the  |   |   |    |      |
|      |      | metad        | hash to be       |   |   |    |      |
|      |      | ata.]{.mark} | provided. Only   |   |   |    |      |
|      |      |              | url or only hash |   |   |    |      |
|      |      |              | is not allowed.\ |   |   |    |      |
|      |      |              | \                |   |   |    |      |
|      |      |              | \--d             |   |   |    |      |
|      |      |              | rep-metadata-url |   |   |    |      |
|      |      |              | TEXT             |   |   |    |      |
|      |      |              | \--dr            |   |   |    |      |
|      |      |              | ep-metadata-hash |   |   |    |      |
|      |      |              | HASH]{.mark}     |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | [\               |   |   |    |      |
|      |      |              | ]{.mark}Failing  |   |   |    |      |
|      |      |              | to provide the   |   |   |    |      |
|      |      |              | right input      |   |   |    |      |
|      |      |              | results in a     |   |   |    |      |
|      |      |              | clear error      |   |   |    |      |
|      |      |              | message that     |   |   |    |      |
|      |      |              | helps the user   |   |   |    |      |
|      |      |              | to identify the  |   |   |    |      |
|      |      |              | problem          |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [When the    | [The anchor is   |   |   |    |      |
|      |      | \--drep-     | included in the  |   |   |    |      |
|      |      | metadata-url | certificate on   |   |   |    |      |
|      |      | and          | the last         |   |   |    |      |
|      |      | \--dr        | p                |   |   |    |      |
|      |      | ep-metadata- | osition:]{.mark} |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      |              | [reg_drep_cert = |   |   |    |      |
|      |      | [are         | (16,             |   |   |    |      |
|      |      | provided,    | drep_credential, |   |   |    |      |
|      |      | the          | coin, anchor /   |   |   |    |      |
|      |      | resulting    | null)]{.mark}    |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | should       |                  |   |   |    |      |
|      |      | include the  |                  |   |   |    |      |
|      |      | url and hash |                  |   |   |    |      |
|      |      | on the       |                  |   |   |    |      |
|      |      | anchor       |                  |   |   |    |      |
|      |      | position,    |                  |   |   |    |      |
|      |      | otherwise    |                  |   |   |    |      |
|      |      | the field is |                  |   |   |    |      |
|      |      | n            |                  |   |   |    |      |
|      |      | ull.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | The flag         |   |   |    |      |
|      |      | \--out-file  | [\--             |   |   |    |      |
|      |      | FILE option  | out-file]{.mark} |   |   |    |      |
|      |      | is mandatory | is mandatory and |   |   |    |      |
|      |      | and used to  | takes the file   |   |   |    |      |
|      |      | specify the  | path and name as |   |   |    |      |
|      |      | file where   | an argument.     |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | generated    | Failure to       |   |   |    |      |
|      |      | DRep         | provide the flag |   |   |    |      |
|      |      | registration | and its argument |   |   |    |      |
|      |      | certificate  | generates an     |   |   |    |      |
|      |      | will be      | exception.       |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | [reg_drep_cert = |   |   |    |      |
|      |      | generates a  | (16,             |   |   |    |      |
|      |      | registration | drep_credential, |   |   |    |      |
|      |      | certificate  | coin, anchor /   |   |   |    |      |
|      |      | compliant    | null)]{.mark}    |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway       |                  |   |   |    |      |
|      |      | cddl]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\           |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Given that the   |   |   |    |      |
|      |      | certificate  | certificate is   |   |   |    |      |
|      |      | should be on | saved, then it   |   |   |    |      |
|      |      | a text       | is in a text     |   |   |    |      |
|      |      | envelope     | envelope format  |   |   |    |      |
|      |      | format,      | consisting of a  |   |   |    |      |
|      |      | similar to   | json object with |   |   |    |      |
|      |      | what we have | type,            |   |   |    |      |
|      |      | for stake    | description and  |   |   |    |      |
|      |      | pools        | cbor hex fields, |   |   |    |      |
|      |      | registration | where:           |   |   |    |      |
|      |      | certific     |                  |   |   |    |      |
|      |      | ates]{.mark} | [{]{.mark}      |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | [\"type\":       |   |   |    |      |
|      |      |              | \"CertificateC   |   |   |    |      |
|      |      |              | onway\",]{.mark} |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | [                |   |   |    |      |
|      |      |              | \"description\": |   |   |    |      |
|      |      |              | \"DRep           |   |   |    |      |
|      |      |              | Registration     |   |   |    |      |
|      |      |              | Certif           |   |   |    |      |
|      |      |              | icate\",]{.mark} |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | [\"cborHex\":    |   |   |    |      |
|      |      |              | \"00             |   |   |    |      |
|      |      |              | 000000\"]{.mark} |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | [}]{.mark}       |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | []{.mark}       |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The feature | Detail Pending   |   |   |    |      |
|      |      | im           |                  |   |   |    |      |
|      |      | plementation |                  |   |   |    |      |
|      |      | should be    |                  |   |   |    |      |
|      |      | well         |                  |   |   |    |      |
|      |      | -documented, |                  |   |   |    |      |
|      |      | providing    |                  |   |   |    |      |
|      |      | clear usage  |                  |   |   |    |      |
|      |      | instructions |                  |   |   |    |      |
|      |      | for the      |                  |   |   |    |      |
|      |      | cardano-cli  |                  |   |   |    |      |
|      |      | conway       |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | drep         |                  |   |   |    |      |
|      |      | registration |                  |   |   |    |      |
|      |      | -certificate |                  |   |   |    |      |
|      |      | comm         |                  |   |   |    |      |
|      |      | and.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | should       |                  |   |   |    |      |
|      |      | handle       |                  |   |   |    |      |
|      |      | errors       |                  |   |   |    |      |
|      |      | gracefully   |                  |   |   |    |      |
|      |      | and provide  |                  |   |   |    |      |
|      |      | helpful      |                  |   |   |    |      |
|      |      | error        |                  |   |   |    |      |
|      |      | messages     |                  |   |   |    |      |
|      |      | when         |                  |   |   |    |      |
|      |      | required     |                  |   |   |    |      |
|      |      | options are  |                  |   |   |    |      |
|      |      | missing or   |                  |   |   |    |      |
|      |      | invalid      |                  |   |   |    |      |
|      |      | inputs are   |                  |   |   |    |      |
|      |      | provi        |                  |   |   |    |      |
|      |      | ded.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As a | [The command | Typing           |   |   |    |      |
| LI11 | DRep | allows the   | cardano-cli      |   |   |    |      |
|      |      | user to      | conway           |   |   |    |      |
|      | I    | provide the  | governance drep  |   |   |    |      |
|      | want | DRep         | retire           |   |   |    |      |
|      | to   | credentials  | ment-certificate |   |   |    |      |
|      | gene | in the       |                  |   |   |    |      |
|      | rate | following    | with accepted    |   |   |    |      |
|      | a    | w            | input parameters |   |   |    |      |
|      | Drep | ays:]{.mark} | will generate a  |   |   |    |      |
|      | re   |              | DRep retirement  |   |   |    |      |
|      | tire | [Using the   | certificate.     |   |   |    |      |
|      | ment | \--drep-veri |                  |   |   |    |      |
|      | (unr | fication-key |                  |   |   |    |      |
|      | egis | STRING       |                  |   |   |    |      |
|      | trat | option to    |                  |   |   |    |      |
|      | ion) | specify the  |                  |   |   |    |      |
|      | cer  | DRep         |                  |   |   |    |      |
|      | tifi | verification |                  |   |   |    |      |
|      | cate | key directly |                  |   |   |    |      |
|      |      | as a         |                  |   |   |    |      |
|      | So   | str          |                  |   |   |    |      |
|      | that | ing.]{.mark} |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  | [Using the   |                  |   |   |    |      |
|      | su   | \--dr        |                  |   |   |    |      |
|      | bmit | ep-verificat |                  |   |   |    |      |
|      | it   | ion-key-file |                  |   |   |    |      |
|      | on a | FILE option  |                  |   |   |    |      |
|      | tra  | to specify   |                  |   |   |    |      |
|      | nsac | the file     |                  |   |   |    |      |
|      | tion | containing   |                  |   |   |    |      |
|      | and  | the DRep     |                  |   |   |    |      |
|      | can  | verification |                  |   |   |    |      |
|      | get  | key.]{.mark} |                  |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | DRep | [Using the   |                  |   |   |    |      |
|      | dep  | \--drep-id   |                  |   |   |    |      |
|      | osit | STRING       |                  |   |   |    |      |
|      | b    | option to    |                  |   |   |    |      |
|      | ack. | specify the  |                  |   |   |    |      |
|      |      | DRep ID      |                  |   |   |    |      |
|      |      | directly as  |                  |   |   |    |      |
|      |      | a            |                  |   |   |    |      |
|      |      | str          |                  |   |   |    |      |
|      |      | ing.]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | cardano-cli  |                  |   |   |    |      |
|      |      | conway       |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | drep         |                  |   |   |    |      |
|      |      | retirement   |                  |   |   |    |      |
|      |      | -certificate |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | The flag         |   |   |    |      |
|      |      | has the      | [\--dep          |   |   |    |      |
|      |      | mandatory    | osit-amt]{.mark} |   |   |    |      |
|      |      | flag         | is mandatory and |   |   |    |      |
|      |      | \-           | takes the        |   |   |    |      |
|      |      | -deposit-amt | deposit amount   |   |   |    |      |
|      |      | to require   | in lovelace as   |   |   |    |      |
|      |      | the user to  | an argument. The |   |   |    |      |
|      |      | provide the  | argument is a    |   |   |    |      |
|      |      | drep         | decimal,         |   |   |    |      |
|      |      | deposited    | providing any    |   |   |    |      |
|      |      | amount that  | other type of    |   |   |    |      |
|      |      | is to be     | input will       |   |   |    |      |
|      |      | returned.\   | result in an     |   |   |    |      |
|      |      | \            | exception (no    |   |   |    |      |
|      |      | Must match   | implicit         |   |   |    |      |
|      |      | the deposit  | conversion)      |   |   |    |      |
|      |      | originally   |                  |   |   |    |      |
|      |      | paid when    | Not providing    |   |   |    |      |
|      |      | registering  | the flag and its |   |   |    |      |
|      |      | as DRep but  | argument         |   |   |    |      |
|      |      | is only      | generates an     |   |   |    |      |
|      |      | checked when | exception.       |   |   |    |      |
|      |      | submitting   |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | transact     |                  |   |   |    |      |
|      |      | ion.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | The flag         |   |   |    |      |
|      |      | \--out-file  | [\--             |   |   |    |      |
|      |      | FILE option  | out-file]{.mark} |   |   |    |      |
|      |      | should be    | is mandatory and |   |   |    |      |
|      |      | mandatory    | takes the file   |   |   |    |      |
|      |      | and used to  | path and name as |   |   |    |      |
|      |      | specify the  | an argument.     |   |   |    |      |
|      |      | file where   |                  |   |   |    |      |
|      |      | the          | Failure to       |   |   |    |      |
|      |      | generated    | provide the flag |   |   |    |      |
|      |      | DRep         | and its argument |   |   |    |      |
|      |      | retirement   | generates an     |   |   |    |      |
|      |      | certificate  | exception.       |   |   |    |      |
|      |      | will be      |                  |   |   |    |      |
|      |      | s            |                  |   |   |    |      |
|      |      | aved]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Given that the   |   |   |    |      |
|      |      | certificate  | certificate is   |   |   |    |      |
|      |      | should be on | saved, then it   |   |   |    |      |
|      |      | a text       | is in a text     |   |   |    |      |
|      |      | envelope     | envelope format  |   |   |    |      |
|      |      | format,      | consisting of a  |   |   |    |      |
|      |      | similar to   | json object with |   |   |    |      |
|      |      | what we have | type,            |   |   |    |      |
|      |      | for stake    | description and  |   |   |    |      |
|      |      | pools        | cbor hex fields, |   |   |    |      |
|      |      | de           | where:           |   |   |    |      |
|      |      | registration |                  |   |   |    |      |
|      |      | certific     | [{]{.mark}      |   |   |    |      |
|      |      | ates]{.mark} |                  |   |   |    |      |
|      |      |              | [\"type\":       |   |   |    |      |
|      |      |              | \"CertificateC   |   |   |    |      |
|      |      |              | onway\",]{.mark} |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | [                |   |   |    |      |
|      |      |              | \"description\": |   |   |    |      |
|      |      |              | \"DRep           |   |   |    |      |
|      |      |              | Retirement       |   |   |    |      |
|      |      |              | Certif           |   |   |    |      |
|      |      |              | icate\",]{.mark} |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | [\"cborHex\":    |   |   |    |      |
|      |      |              | \"00             |   |   |    |      |
|      |      |              | 000000\"]{.mark} |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | [}]{.mark}       |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      |              | []{.mark}       |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The output  | Detail Pending   |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | complies     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl\ |                  |   |   |    |      |
|      |      | \            |                  |   |   |    |      |
|      |      | unr          |                  |   |   |    |      |
|      |      | eg_drep_cert |                  |   |   |    |      |
|      |      | = (17,       |                  |   |   |    |      |
|      |      | drep         |                  |   |   |    |      |
|      |      | _credential, |                  |   |   |    |      |
|      |      | c            |                  |   |   |    |      |
|      |      | oin)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The feature | Detail Pending   |   |   |    |      |
|      |      | im           |                  |   |   |    |      |
|      |      | plementation |                  |   |   |    |      |
|      |      | should be    |                  |   |   |    |      |
|      |      | well         |                  |   |   |    |      |
|      |      | -documented, |                  |   |   |    |      |
|      |      | providing    |                  |   |   |    |      |
|      |      | clear usage  |                  |   |   |    |      |
|      |      | instruct     |                  |   |   |    |      |
|      |      | ions]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | handles      |                  |   |   |    |      |
|      |      | errors       |                  |   |   |    |      |
|      |      | gracefully   |                  |   |   |    |      |
|      |      | and provides |                  |   |   |    |      |
|      |      | helpful      |                  |   |   |    |      |
|      |      | error        |                  |   |   |    |      |
|      |      | messages     |                  |   |   |    |      |
|      |      | when         |                  |   |   |    |      |
|      |      | required     |                  |   |   |    |      |
|      |      | options are  |                  |   |   |    |      |
|      |      | missing or   |                  |   |   |    |      |
|      |      | invalid      |                  |   |   |    |      |
|      |      | inputs are   |                  |   |   |    |      |
|      |      | provi        |                  |   |   |    |      |
|      |      | ded.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As a | [The command | Detail Pending   |   |   |    |      |
| LI12 | Drep | calculates   |                  |   |   |    |      |
|      |      | the blake2b  |                  |   |   |    |      |
|      | I    | 256 hash of  |                  |   |   |    |      |
|      | want | the file     |                  |   |   |    |      |
|      | to   | supplied by  |                  |   |   |    |      |
|      | gene | the          |                  |   |   |    |      |
|      | rate | u            |                  |   |   |    |      |
|      | the  | ser.]{.mark} |                  |   |   |    |      |
|      | hash |              |                  |   |   |    |      |
|      | of   | cardano-cli  |                  |   |   |    |      |
|      | my   | conway       |                  |   |   |    |      |
|      | DRep | governance   |                  |   |   |    |      |
|      | meta | drep         |                  |   |   |    |      |
|      | data | m            |                  |   |   |    |      |
|      |      | etadata-hash |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | su   |              |                  |   |   |    |      |
|      | pply |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | when |              |                  |   |   |    |      |
|      | reg  |              |                  |   |   |    |      |
|      | iste |              |                  |   |   |    |      |
|      | ring |              |                  |   |   |    |      |
|      | as   |              |                  |   |   |    |      |
|      | DRep |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | \--drep-m    |                  |   |   |    |      |
|      |      | etadata-file |                  |   |   |    |      |
|      |      | FILE option  |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | containing   |                  |   |   |    |      |
|      |      | the DRep     |                  |   |   |    |      |
|      |      | metad        |                  |   |   |    |      |
|      |      | ata.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | supports the |                  |   |   |    |      |
|      |      | \--out-file  |                  |   |   |    |      |
|      |      | FILE option  |                  |   |   |    |      |
|      |      | (optional)   |                  |   |   |    |      |
|      |      | to enable    |                  |   |   |    |      |
|      |      | users to     |                  |   |   |    |      |
|      |      | save the     |                  |   |   |    |      |
|      |      | calculated   |                  |   |   |    |      |
|      |      | metadata     |                  |   |   |    |      |
|      |      | hash to the  |                  |   |   |    |      |
|      |      | specified    |                  |   |   |    |      |
|      |      | file. If the |                  |   |   |    |      |
|      |      | flag is not  |                  |   |   |    |      |
|      |      | used, the    |                  |   |   |    |      |
|      |      | hash is      |                  |   |   |    |      |
|      |      | printed to   |                  |   |   |    |      |
|      |      | st           |                  |   |   |    |      |
|      |      | dout]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | handles      |                  |   |   |    |      |
|      |      | errors       |                  |   |   |    |      |
|      |      | gracefully   |                  |   |   |    |      |
|      |      | and provides |                  |   |   |    |      |
|      |      | helpful      |                  |   |   |    |      |
|      |      | error        |                  |   |   |    |      |
|      |      | messages     |                  |   |   |    |      |
|      |      | when         |                  |   |   |    |      |
|      |      | required     |                  |   |   |    |      |
|      |      | options are  |                  |   |   |    |      |
|      |      | missing or   |                  |   |   |    |      |
|      |      | invalid      |                  |   |   |    |      |
|      |      | inputs are   |                  |   |   |    |      |
|      |      | provi        |                  |   |   |    |      |
|      |      | ded.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [The command | Detail Pending   |   |   |    |      |
| LI13 | an   | requires     |                  |   |   |    |      |
|      | ada  | either       |                  |   |   |    |      |
|      | ho   | \--mainnet   |                  |   |   |    |      |
|      | lder | or           |                  |   |   |    |      |
|      |      | \--t         |                  |   |   |    |      |
|      | I    | estnet-magic |                  |   |   |    |      |
|      | want | NATURAL      |                  |   |   |    |      |
|      | to   | option to    |                  |   |   |    |      |
|      | cr   | specify the  |                  |   |   |    |      |
|      | eate | target       |                  |   |   |    |      |
|      | a    | network for  |                  |   |   |    |      |
|      | go   | which the    |                  |   |   |    |      |
|      | vern | governance   |                  |   |   |    |      |
|      | ance | action is    |                  |   |   |    |      |
|      | ac   | gener        |                  |   |   |    |      |
|      | tion | ated]{.mark} |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | upd  | cardano-cli  |                  |   |   |    |      |
|      | ates | conway       |                  |   |   |    |      |
|      | the  | governance   |                  |   |   |    |      |
|      | cons | action       |                  |   |   |    |      |
|      | titu | create-      |                  |   |   |    |      |
|      | tion | constitution |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | s    |              |                  |   |   |    |      |
|      | ubmi |              |                  |   |   |    |      |
|      | tted |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | v    |              |                  |   |   |    |      |
|      | oted |              |                  |   |   |    |      |
|      | by   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | bo   |              |                  |   |   |    |      |
|      | dies |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | the deposit  |                  |   |   |    |      |
|      |      | amount for   |                  |   |   |    |      |
|      |      | submitting   |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | actions via  |                  |   |   |    |      |
|      |      | the flag     |                  |   |   |    |      |
|      |      | *\           |                  |   |   |    |      |
|      |      | --governance |                  |   |   |    |      |
|      |      | -action-depo |                  |   |   |    |      |
|      |      | sit*]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | stake        |                  |   |   |    |      |
|      |      | credential   |                  |   |   |    |      |
|      |      | that will    |                  |   |   |    |      |
|      |      | receive the  |                  |   |   |    |      |
|      |      | deposit      |                  |   |   |    |      |
|      |      | return when  |                  |   |   |    |      |
|      |      | the action   |                  |   |   |    |      |
|      |      | is           |                  |   |   |    |      |
|      |      | enac         |                  |   |   |    |      |
|      |      | ted/expired. |                  |   |   |    |      |
|      |      | It accepts:\ |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\-          |                  |   |   |    |      |
|      |      | -stake-verif |                  |   |   |    |      |
|      |      | ication-key- |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\--stake-   |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | -key]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\           |                  |   |   |    |      |
|      |      | --stake-key- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | allows the   |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | transaction  |                  |   |   |    |      |
|      |      | id and index |                  |   |   |    |      |
|      |      | of the       |                  |   |   |    |      |
|      |      | previously   |                  |   |   |    |      |
|      |      | enacted      |                  |   |   |    |      |
|      |      | action of    |                  |   |   |    |      |
|      |      | this type.   |                  |   |   |    |      |
|      |      | These flags  |                  |   |   |    |      |
|      |      | are optional |                  |   |   |    |      |
|      |      | (but if one  |                  |   |   |    |      |
|      |      | is used the  |                  |   |   |    |      |
|      |      | other one    |                  |   |   |    |      |
|      |      | must be used |                  |   |   |    |      |
|      |      | too) to      |                  |   |   |    |      |
|      |      | support the  |                  |   |   |    |      |
|      |      | very first   |                  |   |   |    |      |
|      |      | action of    |                  |   |   |    |      |
|      |      | this type on |                  |   |   |    |      |
|      |      | the system   |                  |   |   |    |      |
|      |      | which does   |                  |   |   |    |      |
|      |      | not require  |                  |   |   |    |      |
|      |      | information  |                  |   |   |    |      |
|      |      | about        |                  |   |   |    |      |
|      |      | previously   |                  |   |   |    |      |
|      |      | enacted      |                  |   |   |    |      |
|      |      | actions. The |                  |   |   |    |      |
|      |      | flags        |                  |   |   |    |      |
|      |      | are:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\--governa  |                  |   |   |    |      |
|      |      | nce-action-t |                  |   |   |    |      |
|      |      | x-id]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\--governa  |                  |   |   |    |      |
|      |      | nce-action-i |                  |   |   |    |      |
|      |      | ndex]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide an   |                  |   |   |    |      |
|      |      | anchor (url  |                  |   |   |    |      |
|      |      | / hash) of   |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | proposal. A  |                  |   |   |    |      |
|      |      | document     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | proposer     |                  |   |   |    |      |
|      |      | exposes the  |                  |   |   |    |      |
|      |      | reasoning    |                  |   |   |    |      |
|      |      | behind the   |                  |   |   |    |      |
|      |      | proposed     |                  |   |   |    |      |
|      |      | change.\     |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\--anchor   |                  |   |   |    |      |
|      |      | -url]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\--         |                  |   |   |    |      |
|      |      | anchor-data- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide an   |                  |   |   |    |      |
|      |      | anchor (url  |                  |   |   |    |      |
|      |      | / hash) of   |                  |   |   |    |      |
|      |      | the new      |                  |   |   |    |      |
|      |      | co           |                  |   |   |    |      |
|      |      | nstitution.\ |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\--         |                  |   |   |    |      |
|      |      | constitution |                  |   |   |    |      |
|      |      | -url]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\--c        |                  |   |   |    |      |
|      |      | onstitution- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the      |                  |   |   |    |      |
|      |      | mandatory    |                  |   |   |    |      |
|      |      | flag         |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | here the     |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action (the  |                  |   |   |    |      |
|      |      | proposal)    |                  |   |   |    |      |
|      |      | will be      |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Detail Pending   |   |   |    |      |
|      |      | generated    |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action       |                  |   |   |    |      |
|      |      | complies     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl, |                  |   |   |    |      |
|      |      | where:\      |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [propos      |                  |   |   |    |      |
|      |      | al_procedure |                  |   |   |    |      |
|      |      | =]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\[ deposit  |                  |   |   |    |      |
|      |      | :            |                  |   |   |    |      |
|      |      | coin]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | reward_acc   |                  |   |   |    |      |
|      |      | ount]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | gov_ac       |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | an           |                  |   |   |    |      |
|      |      | chor]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\]]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [new_        |                  |   |   |    |      |
|      |      | constitution |                  |   |   |    |      |
|      |      | = (5,        |                  |   |   |    |      |
|      |      | g            |                  |   |   |    |      |
|      |      | ov_action_id |                  |   |   |    |      |
|      |      | / null,      |                  |   |   |    |      |
|      |      | constitut    |                  |   |   |    |      |
|      |      | ion)]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [            |                  |   |   |    |      |
|      |      | constitution |                  |   |   |    |      |
|      |      | =]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\[          |                  |   |   |    |      |
|      |      | an           |                  |   |   |    |      |
|      |      | chor]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | scripthash / |                  |   |   |    |      |
|      |      | null]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\]]{.mark}  |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [The command | Detail Pending   |   |   |    |      |
| LI14 | an   | requires     |                  |   |   |    |      |
|      | ada  | either       |                  |   |   |    |      |
|      | ho   | \--mainnet   |                  |   |   |    |      |
|      | lder | or           |                  |   |   |    |      |
|      |      | \--t         |                  |   |   |    |      |
|      | I    | estnet-magic |                  |   |   |    |      |
|      | want | NATURAL      |                  |   |   |    |      |
|      | to   | option to    |                  |   |   |    |      |
|      | cr   | specify the  |                  |   |   |    |      |
|      | eate | target       |                  |   |   |    |      |
|      | a    | network for  |                  |   |   |    |      |
|      | go   | which the    |                  |   |   |    |      |
|      | vern | action is    |                  |   |   |    |      |
|      | ance | gener        |                  |   |   |    |      |
|      | ac   | ated]{.mark} |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | upd  |              |                  |   |   |    |      |
|      | ates |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | co   |              |                  |   |   |    |      |
|      | nsti |              |                  |   |   |    |      |
|      | tuti |              |                  |   |   |    |      |
|      | onal |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | ommi |              |                  |   |   |    |      |
|      | ttee |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | s    |              |                  |   |   |    |      |
|      | ubmi |              |                  |   |   |    |      |
|      | tted |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | v    |              |                  |   |   |    |      |
|      | oted |              |                  |   |   |    |      |
|      | by   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | bo   |              |                  |   |   |    |      |
|      | dies |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | the deposit  |                  |   |   |    |      |
|      |      | amount for   |                  |   |   |    |      |
|      |      | submitting   |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | actions via  |                  |   |   |    |      |
|      |      | the flag     |                  |   |   |    |      |
|      |      | *\           |                  |   |   |    |      |
|      |      | --governance |                  |   |   |    |      |
|      |      | -action-depo |                  |   |   |    |      |
|      |      | sit*]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | stake        |                  |   |   |    |      |
|      |      | credential   |                  |   |   |    |      |
|      |      | that will    |                  |   |   |    |      |
|      |      | receive the  |                  |   |   |    |      |
|      |      | deposit      |                  |   |   |    |      |
|      |      | return when  |                  |   |   |    |      |
|      |      | the action   |                  |   |   |    |      |
|      |      | is           |                  |   |   |    |      |
|      |      | enac         |                  |   |   |    |      |
|      |      | ted/expired. |                  |   |   |    |      |
|      |      | It accepts:\ |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\-          |                  |   |   |    |      |
|      |      | -stake-verif |                  |   |   |    |      |
|      |      | ication-key- |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\--stake-   |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | -key]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\           |                  |   |   |    |      |
|      |      | --stake-key- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide an   |                  |   |   |    |      |
|      |      | anchor (url  |                  |   |   |    |      |
|      |      | / hash) of   |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | proposal. A  |                  |   |   |    |      |
|      |      | document     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | proposer     |                  |   |   |    |      |
|      |      | exposes the  |                  |   |   |    |      |
|      |      | reasoning    |                  |   |   |    |      |
|      |      | behind the   |                  |   |   |    |      |
|      |      | proposed     |                  |   |   |    |      |
|      |      | change.\     |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\--anchor   |                  |   |   |    |      |
|      |      | -url]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\--         |                  |   |   |    |      |
|      |      | anchor-data- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | offers the   |                  |   |   |    |      |
|      |      | option to    |                  |   |   |    |      |
|      |      | remove many  |                  |   |   |    |      |
|      |      | CC members,  |                  |   |   |    |      |
|      |      | it accepts:\ |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\--remove-c |                  |   |   |    |      |
|      |      | c-cold-verif |                  |   |   |    |      |
|      |      | ication-key- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\--rem      |                  |   |   |    |      |
|      |      | ove-cc-cold- |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | -key]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\--remove-c |                  |   |   |    |      |
|      |      | c-cold-verif |                  |   |   |    |      |
|      |      | ication-key- |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | offers the   |                  |   |   |    |      |
|      |      | option to    |                  |   |   |    |      |
|      |      | add many CC  |                  |   |   |    |      |
|      |      | members.\    |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\--         |                  |   |   |    |      |
|      |      | add-cc-cold- |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | -key]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\--add-c    |                  |   |   |    |      |
|      |      | c-cold-verif |                  |   |   |    |      |
|      |      | ication-key- |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\--add-c    |                  |   |   |    |      |
|      |      | c-cold-verif |                  |   |   |    |      |
|      |      | ication-key- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [When adding | Detail Pending   |   |   |    |      |
|      |      | a new        |                  |   |   |    |      |
|      |      | member, the  |                  |   |   |    |      |
|      |      | command      |                  |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to also |                  |   |   |    |      |
|      |      | provide a    |                  |   |   |    |      |
|      |      | term for     |                  |   |   |    |      |
|      |      | each new     |                  |   |   |    |      |
|      |      | member using |                  |   |   |    |      |
|      |      | the flag     |                  |   |   |    |      |
|      |      | --e          |                  |   |   |    |      |
|      |      | poch]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | allows       |                  |   |   |    |      |
|      |      | proposing a  |                  |   |   |    |      |
|      |      | new quorum   |                  |   |   |    |      |
|      |      | thresh       |                  |   |   |    |      |
|      |      | old:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [When      |                  |   |   |    |      |
|      |      | > adding     |                  |   |   |    |      |
|      |      | > mem        |                  |   |   |    |      |
|      |      | bers]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [When      |                  |   |   |    |      |
|      |      | > removing   |                  |   |   |    |      |
|      |      | > mem        |                  |   |   |    |      |
|      |      | bers]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [As        |                  |   |   |    |      |
|      |      | > standalone |                  |   |   |    |      |
|      |      | > action (no |                  |   |   |    |      |
|      |      | > adds or    |                  |   |   |    |      |
|      |      | > remov      |                  |   |   |    |      |
|      |      | als)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action (the  |                  |   |   |    |      |
|      |      | proposal)    |                  |   |   |    |      |
|      |      | will be      |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Detail Pending   |   |   |    |      |
|      |      | generated    |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action       |                  |   |   |    |      |
|      |      | complies     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl, |                  |   |   |    |      |
|      |      | where:\      |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [propos      |                  |   |   |    |      |
|      |      | al_procedure |                  |   |   |    |      |
|      |      | =]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\[ deposit  |                  |   |   |    |      |
|      |      | :            |                  |   |   |    |      |
|      |      | coin]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | reward_acc   |                  |   |   |    |      |
|      |      | ount]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | gov_ac       |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | an           |                  |   |   |    |      |
|      |      | chor]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\]]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [upda        |                  |   |   |    |      |
|      |      | te_committee |                  |   |   |    |      |
|      |      | = (4,        |                  |   |   |    |      |
|      |      | g            |                  |   |   |    |      |
|      |      | ov_action_id |                  |   |   |    |      |
|      |      | / null,      |                  |   |   |    |      |
|      |      | set\<comm    |                  |   |   |    |      |
|      |      | ittee_cold_c |                  |   |   |    |      |
|      |      | redential\>, |                  |   |   |    |      |
|      |      | {            |                  |   |   |    |      |
|      |      | c            |                  |   |   |    |      |
|      |      | ommittee_col |                  |   |   |    |      |
|      |      | d_credential |                  |   |   |    |      |
|      |      | =\> epoch }, |                  |   |   |    |      |
|      |      | unit_inter   |                  |   |   |    |      |
|      |      | val)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [The command | Detail Pending   |   |   |    |      |
| LI15 | an   | requires     |                  |   |   |    |      |
|      | ada  | either       |                  |   |   |    |      |
|      | ho   | \--mainnet   |                  |   |   |    |      |
|      | lder | or           |                  |   |   |    |      |
|      |      | \--t         |                  |   |   |    |      |
|      | I    | estnet-magic |                  |   |   |    |      |
|      | want | NATURAL      |                  |   |   |    |      |
|      | to   | option to    |                  |   |   |    |      |
|      | cr   | specify the  |                  |   |   |    |      |
|      | eate | target       |                  |   |   |    |      |
|      | a    | network for  |                  |   |   |    |      |
|      | go   | which the    |                  |   |   |    |      |
|      | vern | action is    |                  |   |   |    |      |
|      | ance | gener        |                  |   |   |    |      |
|      | ac   | ated]{.mark} |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | with |              |                  |   |   |    |      |
|      | draw |              |                  |   |   |    |      |
|      | f    |              |                  |   |   |    |      |
|      | unds |              |                  |   |   |    |      |
|      | from |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | trea |              |                  |   |   |    |      |
|      | sury |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | s    |              |                  |   |   |    |      |
|      | ubmi |              |                  |   |   |    |      |
|      | tted |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | v    |              |                  |   |   |    |      |
|      | oted |              |                  |   |   |    |      |
|      | by   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | bo   |              |                  |   |   |    |      |
|      | dies |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | car  |              |                  |   |   |    |      |
|      | dano |              |                  |   |   |    |      |
|      | -cli |              |                  |   |   |    |      |
|      | co   |              |                  |   |   |    |      |
|      | nway |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | ac   |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | cr   |              |                  |   |   |    |      |
|      | eate |              |                  |   |   |    |      |
|      | -tre |              |                  |   |   |    |      |
|      | asur |              |                  |   |   |    |      |
|      | y-wi |              |                  |   |   |    |      |
|      | thdr |              |                  |   |   |    |      |
|      | awal |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | the deposit  |                  |   |   |    |      |
|      |      | amount for   |                  |   |   |    |      |
|      |      | submitting   |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | actions via  |                  |   |   |    |      |
|      |      | the flag     |                  |   |   |    |      |
|      |      | *\           |                  |   |   |    |      |
|      |      | --governance |                  |   |   |    |      |
|      |      | -action-depo |                  |   |   |    |      |
|      |      | sit*]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | stake        |                  |   |   |    |      |
|      |      | credential   |                  |   |   |    |      |
|      |      | that will    |                  |   |   |    |      |
|      |      | receive the  |                  |   |   |    |      |
|      |      | deposit      |                  |   |   |    |      |
|      |      | return when  |                  |   |   |    |      |
|      |      | the action   |                  |   |   |    |      |
|      |      | is           |                  |   |   |    |      |
|      |      | enac         |                  |   |   |    |      |
|      |      | ted/expired. |                  |   |   |    |      |
|      |      | It accepts:\ |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [\-        |                  |   |   |    |      |
|      |      | -stake-verif |                  |   |   |    |      |
|      |      | ication-key- |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\--stake- |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | -key]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\         |                  |   |   |    |      |
|      |      | --stake-key- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide an   |                  |   |   |    |      |
|      |      | anchor (url  |                  |   |   |    |      |
|      |      | / hash) of   |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | proposal. A  |                  |   |   |    |      |
|      |      | document     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | proposer     |                  |   |   |    |      |
|      |      | exposes the  |                  |   |   |    |      |
|      |      | reasoning    |                  |   |   |    |      |
|      |      | behind the   |                  |   |   |    |      |
|      |      | proposed     |                  |   |   |    |      |
|      |      | change.\     |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [\--anchor |                  |   |   |    |      |
|      |      | -url]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\--       |                  |   |   |    |      |
|      |      | anchor-data- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | stake        |                  |   |   |    |      |
|      |      | credential   |                  |   |   |    |      |
|      |      | that will    |                  |   |   |    |      |
|      |      | receive the  |                  |   |   |    |      |
|      |      | funds if the |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action is    |                  |   |   |    |      |
|      |      | ratified. It |                  |   |   |    |      |
|      |      | accepts:\    |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [\-        |                  |   |   |    |      |
|      |      | -stake-verif |                  |   |   |    |      |
|      |      | ication-key- |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\--stake- |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | -key]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\--sta    |                  |   |   |    |      |
|      |      | ke-key-hash\ |                  |   |   |    |      |
|      |      | > ]{.mark}   |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Requires    | Detail Pending   |   |   |    |      |
|      |      | the user to  |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | amount in    |                  |   |   |    |      |
|      |      | lovelace     |                  |   |   |    |      |
|      |      | that will be |                  |   |   |    |      |
|      |      | transferred  |                  |   |   |    |      |
|      |      | from the     |                  |   |   |    |      |
|      |      | treasury to  |                  |   |   |    |      |
|      |      | the stake    |                  |   |   |    |      |
|      |      | credential   |                  |   |   |    |      |
|      |      | if the       |                  |   |   |    |      |
|      |      | action is    |                  |   |   |    |      |
|      |      | ratif        |                  |   |   |    |      |
|      |      | ied.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action (the  |                  |   |   |    |      |
|      |      | proposal)    |                  |   |   |    |      |
|      |      | will be      |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Detail Pending   |   |   |    |      |
|      |      | generated    |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action       |                  |   |   |    |      |
|      |      | complies     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl, |                  |   |   |    |      |
|      |      | wh           |                  |   |   |    |      |
|      |      | ere:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [propos      |                  |   |   |    |      |
|      |      | al_procedure |                  |   |   |    |      |
|      |      | =]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\[ deposit  |                  |   |   |    |      |
|      |      | :            |                  |   |   |    |      |
|      |      | coin]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | reward_acc   |                  |   |   |    |      |
|      |      | ount]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | gov_ac       |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | an           |                  |   |   |    |      |
|      |      | chor]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\]]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [tre         |                  |   |   |    |      |
|      |      | asury_withdr |                  |   |   |    |      |
|      |      | awals_action |                  |   |   |    |      |
|      |      | = (2, {      |                  |   |   |    |      |
|      |      | re           |                  |   |   |    |      |
|      |      | ward_account |                  |   |   |    |      |
|      |      | =\> coin     |                  |   |   |    |      |
|      |      | })]{.mark}   |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [The command | Detail Pending   |   |   |    |      |
| LI16 | an   | requires     |                  |   |   |    |      |
|      | ada  | either       |                  |   |   |    |      |
|      | ho   | \--mainnet   |                  |   |   |    |      |
|      | lder | or           |                  |   |   |    |      |
|      |      | \--t         |                  |   |   |    |      |
|      | I    | estnet-magic |                  |   |   |    |      |
|      | want | NATURAL      |                  |   |   |    |      |
|      | to   | option to    |                  |   |   |    |      |
|      | cr   | specify the  |                  |   |   |    |      |
|      | eate | target       |                  |   |   |    |      |
|      | an   | network for  |                  |   |   |    |      |
|      | info | which the    |                  |   |   |    |      |
|      | go   | action is    |                  |   |   |    |      |
|      | vern | genera       |                  |   |   |    |      |
|      | ance | ted.]{.mark} |                  |   |   |    |      |
|      | ac   |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | s    |              |                  |   |   |    |      |
|      | ubmi |              |                  |   |   |    |      |
|      | tted |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | v    |              |                  |   |   |    |      |
|      | oted |              |                  |   |   |    |      |
|      | by   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | bo   |              |                  |   |   |    |      |
|      | dies |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | car  |              |                  |   |   |    |      |
|      | dano |              |                  |   |   |    |      |
|      | -cli |              |                  |   |   |    |      |
|      | co   |              |                  |   |   |    |      |
|      | nway |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | ac   |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | cre  |              |                  |   |   |    |      |
|      | ate- |              |                  |   |   |    |      |
|      | info |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | the deposit  |                  |   |   |    |      |
|      |      | amount for   |                  |   |   |    |      |
|      |      | submitting   |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | actions via  |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | mandatory    |                  |   |   |    |      |
|      |      | flag         |                  |   |   |    |      |
|      |      | *\           |                  |   |   |    |      |
|      |      | --governance |                  |   |   |    |      |
|      |      | -action-depo |                  |   |   |    |      |
|      |      | sit*]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | stake        |                  |   |   |    |      |
|      |      | credential   |                  |   |   |    |      |
|      |      | that will    |                  |   |   |    |      |
|      |      | receive the  |                  |   |   |    |      |
|      |      | deposit      |                  |   |   |    |      |
|      |      | return when  |                  |   |   |    |      |
|      |      | the action   |                  |   |   |    |      |
|      |      | is           |                  |   |   |    |      |
|      |      | enac         |                  |   |   |    |      |
|      |      | ted/expired. |                  |   |   |    |      |
|      |      | It accepts:\ |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [\-        |                  |   |   |    |      |
|      |      | -stake-verif |                  |   |   |    |      |
|      |      | ication-key- |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\--stake- |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | -key]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\         |                  |   |   |    |      |
|      |      | --stake-key- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide an   |                  |   |   |    |      |
|      |      | anchor (url  |                  |   |   |    |      |
|      |      | / hash) of   |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | proposal. A  |                  |   |   |    |      |
|      |      | document     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | proposer     |                  |   |   |    |      |
|      |      | exposes the  |                  |   |   |    |      |
|      |      | reasoning    |                  |   |   |    |      |
|      |      | behind the   |                  |   |   |    |      |
|      |      | proposed     |                  |   |   |    |      |
|      |      | change.\     |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [\--anchor |                  |   |   |    |      |
|      |      | -url]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\--       |                  |   |   |    |      |
|      |      | anchor-data- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action (the  |                  |   |   |    |      |
|      |      | proposal)    |                  |   |   |    |      |
|      |      | will be      |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Detail Pending   |   |   |    |      |
|      |      | generated    |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action       |                  |   |   |    |      |
|      |      | complies     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl, |                  |   |   |    |      |
|      |      | wh           |                  |   |   |    |      |
|      |      | ere:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [propos      |                  |   |   |    |      |
|      |      | al_procedure |                  |   |   |    |      |
|      |      | =]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\[ deposit  |                  |   |   |    |      |
|      |      | :            |                  |   |   |    |      |
|      |      | coin]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | reward_acc   |                  |   |   |    |      |
|      |      | ount]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | gov_ac       |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | an           |                  |   |   |    |      |
|      |      | chor]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\]]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [info_action |                  |   |   |    |      |
|      |      | = 6]{.mark}  |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [The command | Detail Pending   |   |   |    |      |
| LI17 | an   | requires     |                  |   |   |    |      |
|      | ada  | either       |                  |   |   |    |      |
|      | ho   | \--mainnet   |                  |   |   |    |      |
|      | lder | or           |                  |   |   |    |      |
|      |      | \--t         |                  |   |   |    |      |
|      | I    | estnet-magic |                  |   |   |    |      |
|      | want | NATURAL      |                  |   |   |    |      |
|      | to   | option to    |                  |   |   |    |      |
|      | cr   | specify the  |                  |   |   |    |      |
|      | eate | target       |                  |   |   |    |      |
|      | a    | network for  |                  |   |   |    |      |
|      | go   | which the    |                  |   |   |    |      |
|      | vern | DRep         |                  |   |   |    |      |
|      | ance | registration |                  |   |   |    |      |
|      | ac   | certificate  |                  |   |   |    |      |
|      | tion | is           |                  |   |   |    |      |
|      | to   | genera       |                  |   |   |    |      |
|      | up   | ted.]{.mark} |                  |   |   |    |      |
|      | date |              |                  |   |   |    |      |
|      | prot |              |                  |   |   |    |      |
|      | ocol |              |                  |   |   |    |      |
|      | pa   |              |                  |   |   |    |      |
|      | rame |              |                  |   |   |    |      |
|      | ters |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | s    |              |                  |   |   |    |      |
|      | ubmi |              |                  |   |   |    |      |
|      | tted |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | v    |              |                  |   |   |    |      |
|      | oted |              |                  |   |   |    |      |
|      | by   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | bo   |              |                  |   |   |    |      |
|      | dies |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | car  |              |                  |   |   |    |      |
|      | dano |              |                  |   |   |    |      |
|      | -cli |              |                  |   |   |    |      |
|      | co   |              |                  |   |   |    |      |
|      | nway |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | ac   |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | reat |              |                  |   |   |    |      |
|      | e-pr |              |                  |   |   |    |      |
|      | otoc |              |                  |   |   |    |      |
|      | ol-p |              |                  |   |   |    |      |
|      | aram |              |                  |   |   |    |      |
|      | eter |              |                  |   |   |    |      |
|      | s-up |              |                  |   |   |    |      |
|      | date |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | the deposit  |                  |   |   |    |      |
|      |      | amount for   |                  |   |   |    |      |
|      |      | submitting   |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | actions via  |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | mandatory    |                  |   |   |    |      |
|      |      | flag         |                  |   |   |    |      |
|      |      | *\           |                  |   |   |    |      |
|      |      | --governance |                  |   |   |    |      |
|      |      | -action-depo |                  |   |   |    |      |
|      |      | sit*]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | stake        |                  |   |   |    |      |
|      |      | credential   |                  |   |   |    |      |
|      |      | that will    |                  |   |   |    |      |
|      |      | receive the  |                  |   |   |    |      |
|      |      | deposit      |                  |   |   |    |      |
|      |      | return when  |                  |   |   |    |      |
|      |      | the action   |                  |   |   |    |      |
|      |      | is           |                  |   |   |    |      |
|      |      | enac         |                  |   |   |    |      |
|      |      | ted/expired. |                  |   |   |    |      |
|      |      | It accepts:\ |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [\-        |                  |   |   |    |      |
|      |      | -stake-verif |                  |   |   |    |      |
|      |      | ication-key- |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\--stake- |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | -key]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\         |                  |   |   |    |      |
|      |      | --stake-key- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | allows the   |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | transaction  |                  |   |   |    |      |
|      |      | id and index |                  |   |   |    |      |
|      |      | of the       |                  |   |   |    |      |
|      |      | previously   |                  |   |   |    |      |
|      |      | enacted      |                  |   |   |    |      |
|      |      | action of    |                  |   |   |    |      |
|      |      | this type.   |                  |   |   |    |      |
|      |      | These flags  |                  |   |   |    |      |
|      |      | are optional |                  |   |   |    |      |
|      |      | (but if one  |                  |   |   |    |      |
|      |      | is used the  |                  |   |   |    |      |
|      |      | other one    |                  |   |   |    |      |
|      |      | must be used |                  |   |   |    |      |
|      |      | too) to      |                  |   |   |    |      |
|      |      | support the  |                  |   |   |    |      |
|      |      | very first   |                  |   |   |    |      |
|      |      | action of    |                  |   |   |    |      |
|      |      | this type on |                  |   |   |    |      |
|      |      | the system   |                  |   |   |    |      |
|      |      | which does   |                  |   |   |    |      |
|      |      | not require  |                  |   |   |    |      |
|      |      | information  |                  |   |   |    |      |
|      |      | about        |                  |   |   |    |      |
|      |      | previously   |                  |   |   |    |      |
|      |      | enacted      |                  |   |   |    |      |
|      |      | actions. The |                  |   |   |    |      |
|      |      | flags        |                  |   |   |    |      |
|      |      | are:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  [\--governa |                  |   |   |    |      |
|      |      | nce-action-t |                  |   |   |    |      |
|      |      | x-id]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  [\--governa |                  |   |   |    |      |
|      |      | nce-action-i |                  |   |   |    |      |
|      |      | ndex]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide an   |                  |   |   |    |      |
|      |      | anchor (url  |                  |   |   |    |      |
|      |      | / hash) of   |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | proposal. A  |                  |   |   |    |      |
|      |      | document     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | proposer     |                  |   |   |    |      |
|      |      | exposes the  |                  |   |   |    |      |
|      |      | reasoning    |                  |   |   |    |      |
|      |      | behind the   |                  |   |   |    |      |
|      |      | proposed     |                  |   |   |    |      |
|      |      | change.\     |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [\--anchor |                  |   |   |    |      |
|      |      | -url]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\--       |                  |   |   |    |      |
|      |      | anchor-data- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | includes     |                  |   |   |    |      |
|      |      | dedicated    |                  |   |   |    |      |
|      |      | flags to     |                  |   |   |    |      |
|      |      | reference    |                  |   |   |    |      |
|      |      | the protocol |                  |   |   |    |      |
|      |      | parameter    |                  |   |   |    |      |
|      |      | that the     |                  |   |   |    |      |
|      |      | user is      |                  |   |   |    |      |
|      |      | attempting   |                  |   |   |    |      |
|      |      | to modify.   |                  |   |   |    |      |
|      |      | The          |                  |   |   |    |      |
|      |      | parameters   |                  |   |   |    |      |
|      |      | that can be  |                  |   |   |    |      |
|      |      | included in  |                  |   |   |    |      |
|      |      | this type of |                  |   |   |    |      |
|      |      | proposal     |                  |   |   |    |      |
|      |      | are:\        |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [The network |                  |   |   |    |      |
|      |      | group        |                  |   |   |    |      |
|      |      | consists     |                  |   |   |    |      |
|      |      | of:]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [maximum   |                  |   |   |    |      |
|      |      | > block body |                  |   |   |    |      |
|      |      | > size       |                  |   |   |    |      |
|      |      | > (maxBBS    |                  |   |   |    |      |
|      |      | ize)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [maximum   |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  transaction |                  |   |   |    |      |
|      |      | > size       |                  |   |   |    |      |
|      |      | > (maxTxS    |                  |   |   |    |      |
|      |      | ize)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [maximum   |                  |   |   |    |      |
|      |      | > block      |                  |   |   |    |      |
|      |      | > header     |                  |   |   |    |      |
|      |      | > size       |                  |   |   |    |      |
|      |      | > (maxBHS    |                  |   |   |    |      |
|      |      | ize)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [maximum   |                  |   |   |    |      |
|      |      | > size of a  |                  |   |   |    |      |
|      |      | > serialized |                  |   |   |    |      |
|      |      | > asset      |                  |   |   |    |      |
|      |      | > value      |                  |   |   |    |      |
|      |      | > (maxValS   |                  |   |   |    |      |
|      |      | ize)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [maximum   |                  |   |   |    |      |
|      |      | > script     |                  |   |   |    |      |
|      |      | > execution  |                  |   |   |    |      |
|      |      | > units in a |                  |   |   |    |      |
|      |      | > single     |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  transaction |                  |   |   |    |      |
|      |      | > (maxTxExUn |                  |   |   |    |      |
|      |      | its)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [maximum   |                  |   |   |    |      |
|      |      | > script     |                  |   |   |    |      |
|      |      | > execution  |                  |   |   |    |      |
|      |      | > units in a |                  |   |   |    |      |
|      |      | > single     |                  |   |   |    |      |
|      |      | > block      |                  |   |   |    |      |
|      |      | > (          |                  |   |   |    |      |
|      |      | maxBlockExUn |                  |   |   |    |      |
|      |      | its)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [maximum   |                  |   |   |    |      |
|      |      | > number of  |                  |   |   |    |      |
|      |      | > collateral |                  |   |   |    |      |
|      |      | > inputs     |                  |   |   |    |      |
|      |      | > (maxC      |                  |   |   |    |      |
|      |      | ollateralInp |                  |   |   |    |      |
|      |      | uts)]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [The         |                  |   |   |    |      |
|      |      | economic     |                  |   |   |    |      |
|      |      | group        |                  |   |   |    |      |
|      |      | consists     |                  |   |   |    |      |
|      |      | of:]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [minimum   |                  |   |   |    |      |
|      |      | > fee        |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  coefficient |                  |   |   |    |      |
|      |      | > (minF      |                  |   |   |    |      |
|      |      | eeA)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [minimum   |                  |   |   |    |      |
|      |      | > fee        |                  |   |   |    |      |
|      |      | > constant   |                  |   |   |    |      |
|      |      | > (minF      |                  |   |   |    |      |
|      |      | eeB)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  [delegation |                  |   |   |    |      |
|      |      | > key        |                  |   |   |    |      |
|      |      | > Lovelace   |                  |   |   |    |      |
|      |      | > deposit    |                  |   |   |    |      |
|      |      | > (keyDepo   |                  |   |   |    |      |
|      |      | sit)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [pool      |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | registration |                  |   |   |    |      |
|      |      | > Lovelace   |                  |   |   |    |      |
|      |      | > deposit    |                  |   |   |    |      |
|      |      | > (poolDepo  |                  |   |   |    |      |
|      |      | sit)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [monetary  |                  |   |   |    |      |
|      |      | > expansion  |                  |   |   |    |      |
|      |      | > (          |                  |   |   |    |      |
|      |      | rho)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [treasury  |                  |   |   |    |      |
|      |      | > expansion  |                  |   |   |    |      |
|      |      | > (          |                  |   |   |    |      |
|      |      | tau)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [minimum   |                  |   |   |    |      |
|      |      | > fixed      |                  |   |   |    |      |
|      |      | > rewards    |                  |   |   |    |      |
|      |      | > cut for    |                  |   |   |    |      |
|      |      | > pools      |                  |   |   |    |      |
|      |      | > (minPoolC  |                  |   |   |    |      |
|      |      | ost)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [minimum   |                  |   |   |    |      |
|      |      | > Lovelace   |                  |   |   |    |      |
|      |      | > deposit    |                  |   |   |    |      |
|      |      | > per byte   |                  |   |   |    |      |
|      |      | > of         |                  |   |   |    |      |
|      |      | > serialized |                  |   |   |    |      |
|      |      | > UTxO       |                  |   |   |    |      |
|      |      | > (c         |                  |   |   |    |      |
|      |      | oinsPerUTxOB |                  |   |   |    |      |
|      |      | yte)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [prices of |                  |   |   |    |      |
|      |      | > Plutus     |                  |   |   |    |      |
|      |      | > execution  |                  |   |   |    |      |
|      |      | > units      |                  |   |   |    |      |
|      |      | > (pri       |                  |   |   |    |      |
|      |      | ces)]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [The         |                  |   |   |    |      |
|      |      | technical    |                  |   |   |    |      |
|      |      | group        |                  |   |   |    |      |
|      |      | consists     |                  |   |   |    |      |
|      |      | of:]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [pool      |                  |   |   |    |      |
|      |      | > pledge     |                  |   |   |    |      |
|      |      | > influence  |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | (a0)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [pool      |                  |   |   |    |      |
|      |      | > retirement |                  |   |   |    |      |
|      |      | > maximum    |                  |   |   |    |      |
|      |      | > epoch      |                  |   |   |    |      |
|      |      | > (e         |                  |   |   |    |      |
|      |      | Max)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [desired   |                  |   |   |    |      |
|      |      | > number of  |                  |   |   |    |      |
|      |      | > pools      |                  |   |   |    |      |
|      |      | > (n         |                  |   |   |    |      |
|      |      | Opt)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [Plutus    |                  |   |   |    |      |
|      |      | > execution  |                  |   |   |    |      |
|      |      | > cost       |                  |   |   |    |      |
|      |      | > models     |                  |   |   |    |      |
|      |      | > (costMod   |                  |   |   |    |      |
|      |      | els)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  [proportion |                  |   |   |    |      |
|      |      | > of         |                  |   |   |    |      |
|      |      | > collateral |                  |   |   |    |      |
|      |      | > needed for |                  |   |   |    |      |
|      |      | > scripts    |                  |   |   |    |      |
|      |      | > (colla     |                  |   |   |    |      |
|      |      | teralPercent |                  |   |   |    |      |
|      |      | age)]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [The         |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | group        |                  |   |   |    |      |
|      |      | consists of  |                  |   |   |    |      |
|      |      | all the new  |                  |   |   |    |      |
|      |      | protocol     |                  |   |   |    |      |
|      |      | parameters   |                  |   |   |    |      |
|      |      | that are     |                  |   |   |    |      |
|      |      | introduced   |                  |   |   |    |      |
|      |      | in this      |                  |   |   |    |      |
|      |      | CIP:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  [governance |                  |   |   |    |      |
|      |      | > voting     |                  |   |   |    |      |
|      |      | > thresh     |                  |   |   |    |      |
|      |      | olds]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [dRep      |                  |   |   |    |      |
|      |      | VotingThresh |                  |   |   |    |      |
|      |      | olds]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [dvtCommi  |                  |   |   |    |      |
|      |      | tteeNoConfid |                  |   |   |    |      |
|      |      | ence]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [dv        |                  |   |   |    |      |
|      |      | tCommitteeNo |                  |   |   |    |      |
|      |      | rmal]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [dvtHa     |                  |   |   |    |      |
|      |      | rdForkInitia |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [dvtMo     |                  |   |   |    |      |
|      |      | tionNoConfid |                  |   |   |    |      |
|      |      | ence]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [dv        |                  |   |   |    |      |
|      |      | tPPEconomicG |                  |   |   |    |      |
|      |      | roup]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [dvtPPGovG |                  |   |   |    |      |
|      |      | roup]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [d         |                  |   |   |    |      |
|      |      | vtPPNetworkG |                  |   |   |    |      |
|      |      | roup]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [dvt       |                  |   |   |    |      |
|      |      | PPTechnicalG |                  |   |   |    |      |
|      |      | roup]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [dvtTr     |                  |   |   |    |      |
|      |      | easuryWithdr |                  |   |   |    |      |
|      |      | awal]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [dvtUpda   |                  |   |   |    |      |
|      |      | teToConstitu |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [pool      |                  |   |   |    |      |
|      |      | VotingThresh |                  |   |   |    |      |
|      |      | olds]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [pvtCommi  |                  |   |   |    |      |
|      |      | tteeNoConfid |                  |   |   |    |      |
|      |      | ence]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [pv        |                  |   |   |    |      |
|      |      | tCommitteeNo |                  |   |   |    |      |
|      |      | rmal]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [pvtHa     |                  |   |   |    |      |
|      |      | rdForkInitia |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [pvtMo     |                  |   |   |    |      |
|      |      | tionNoConfid |                  |   |   |    |      |
|      |      | ence]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  [governance |                  |   |   |    |      |
|      |      | > action     |                  |   |   |    |      |
|      |      | > maximum    |                  |   |   |    |      |
|      |      | > lifetime   |                  |   |   |    |      |
|      |      | > in epochs  |                  |   |   |    |      |
|      |      | > (go        |                  |   |   |    |      |
|      |      | vActionLifet |                  |   |   |    |      |
|      |      | ime)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  [governance |                  |   |   |    |      |
|      |      | > action     |                  |   |   |    |      |
|      |      | > deposit    |                  |   |   |    |      |
|      |      | > (g         |                  |   |   |    |      |
|      |      | ovActionDepo |                  |   |   |    |      |
|      |      | sit)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [DRep      |                  |   |   |    |      |
|      |      | > deposit    |                  |   |   |    |      |
|      |      | > amount     |                  |   |   |    |      |
|      |      | > (drepDepo  |                  |   |   |    |      |
|      |      | sit)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [DRep      |                  |   |   |    |      |
|      |      | > activity   |                  |   |   |    |      |
|      |      | > period in  |                  |   |   |    |      |
|      |      | > epochs     |                  |   |   |    |      |
|      |      | > (drepActiv |                  |   |   |    |      |
|      |      | ity)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [minimal   |                  |   |   |    |      |
|      |      | > co         |                  |   |   |    |      |
|      |      | nstitutional |                  |   |   |    |      |
|      |      | > committee  |                  |   |   |    |      |
|      |      | > size       |                  |   |   |    |      |
|      |      | > (ccMinS    |                  |   |   |    |      |
|      |      | ize)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [maximum   |                  |   |   |    |      |
|      |      | > term       |                  |   |   |    |      |
|      |      | > length (in |                  |   |   |    |      |
|      |      | > epochs)    |                  |   |   |    |      |
|      |      | > for the    |                  |   |   |    |      |
|      |      | > co         |                  |   |   |    |      |
|      |      | nstitutional |                  |   |   |    |      |
|      |      | > committee  |                  |   |   |    |      |
|      |      | > members    |                  |   |   |    |      |
|      |      | > (          |                  |   |   |    |      |
|      |      | ccMaxTermLen |                  |   |   |    |      |
|      |      | gth)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action (the  |                  |   |   |    |      |
|      |      | proposal)    |                  |   |   |    |      |
|      |      | will be      |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Detail Pending   |   |   |    |      |
|      |      | generated    |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action       |                  |   |   |    |      |
|      |      | complies     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl, |                  |   |   |    |      |
|      |      | wh           |                  |   |   |    |      |
|      |      | ere:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [propos      |                  |   |   |    |      |
|      |      | al_procedure |                  |   |   |    |      |
|      |      | =]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\[ deposit  |                  |   |   |    |      |
|      |      | :            |                  |   |   |    |      |
|      |      | coin]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | reward_acc   |                  |   |   |    |      |
|      |      | ount]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | gov_ac       |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | an           |                  |   |   |    |      |
|      |      | chor]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\]]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [parameter_c |                  |   |   |    |      |
|      |      | hange_action |                  |   |   |    |      |
|      |      | = (0,        |                  |   |   |    |      |
|      |      | g            |                  |   |   |    |      |
|      |      | ov_action_id |                  |   |   |    |      |
|      |      | / null,      |                  |   |   |    |      |
|      |      | protoc       |                  |   |   |    |      |
|      |      | ol_param_upd |                  |   |   |    |      |
|      |      | ate)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [The command | Detail Pending   |   |   |    |      |
| LI18 | an   | requires     |                  |   |   |    |      |
|      | ada  | either       |                  |   |   |    |      |
|      | ho   | \--mainnet   |                  |   |   |    |      |
|      | lder | or           |                  |   |   |    |      |
|      |      | \--t         |                  |   |   |    |      |
|      | I    | estnet-magic |                  |   |   |    |      |
|      | want | NATURAL      |                  |   |   |    |      |
|      | to   | option to    |                  |   |   |    |      |
|      | cr   | specify the  |                  |   |   |    |      |
|      | eate | target       |                  |   |   |    |      |
|      | a    | network for  |                  |   |   |    |      |
|      | n    | which the    |                  |   |   |    |      |
|      | o-co | action is    |                  |   |   |    |      |
|      | nfid | genera       |                  |   |   |    |      |
|      | ence | ted.]{.mark} |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | ac   |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | s    |              |                  |   |   |    |      |
|      | ubmi |              |                  |   |   |    |      |
|      | tted |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | v    |              |                  |   |   |    |      |
|      | oted |              |                  |   |   |    |      |
|      | by   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | bo   |              |                  |   |   |    |      |
|      | dies |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | car  |              |                  |   |   |    |      |
|      | dano |              |                  |   |   |    |      |
|      | -cli |              |                  |   |   |    |      |
|      | co   |              |                  |   |   |    |      |
|      | nway |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | ac   |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | crea |              |                  |   |   |    |      |
|      | te-n |              |                  |   |   |    |      |
|      | o-co |              |                  |   |   |    |      |
|      | nfid |              |                  |   |   |    |      |
|      | ence |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | the deposit  |                  |   |   |    |      |
|      |      | amount for   |                  |   |   |    |      |
|      |      | submitting   |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | actions via  |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | mandatory    |                  |   |   |    |      |
|      |      | flag         |                  |   |   |    |      |
|      |      | *\           |                  |   |   |    |      |
|      |      | --governance |                  |   |   |    |      |
|      |      | -action-depo |                  |   |   |    |      |
|      |      | sit*]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | stake        |                  |   |   |    |      |
|      |      | credential   |                  |   |   |    |      |
|      |      | that will    |                  |   |   |    |      |
|      |      | receive the  |                  |   |   |    |      |
|      |      | deposit      |                  |   |   |    |      |
|      |      | return when  |                  |   |   |    |      |
|      |      | the action   |                  |   |   |    |      |
|      |      | is           |                  |   |   |    |      |
|      |      | enac         |                  |   |   |    |      |
|      |      | ted/expired. |                  |   |   |    |      |
|      |      | It accepts:\ |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [\-        |                  |   |   |    |      |
|      |      | -stake-verif |                  |   |   |    |      |
|      |      | ication-key- |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\--stake- |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | -key]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\         |                  |   |   |    |      |
|      |      | --stake-key- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | allows the   |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | transaction  |                  |   |   |    |      |
|      |      | id and index |                  |   |   |    |      |
|      |      | of the       |                  |   |   |    |      |
|      |      | previously   |                  |   |   |    |      |
|      |      | enacted      |                  |   |   |    |      |
|      |      | action of    |                  |   |   |    |      |
|      |      | this type.   |                  |   |   |    |      |
|      |      | These flags  |                  |   |   |    |      |
|      |      | are optional |                  |   |   |    |      |
|      |      | (but if one  |                  |   |   |    |      |
|      |      | is used the  |                  |   |   |    |      |
|      |      | other one    |                  |   |   |    |      |
|      |      | must be used |                  |   |   |    |      |
|      |      | too) to      |                  |   |   |    |      |
|      |      | support the  |                  |   |   |    |      |
|      |      | very first   |                  |   |   |    |      |
|      |      | action of    |                  |   |   |    |      |
|      |      | this type on |                  |   |   |    |      |
|      |      | the system   |                  |   |   |    |      |
|      |      | which does   |                  |   |   |    |      |
|      |      | not require  |                  |   |   |    |      |
|      |      | information  |                  |   |   |    |      |
|      |      | about        |                  |   |   |    |      |
|      |      | previously   |                  |   |   |    |      |
|      |      | enacted      |                  |   |   |    |      |
|      |      | actions. The |                  |   |   |    |      |
|      |      | flags        |                  |   |   |    |      |
|      |      | are:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  [\--governa |                  |   |   |    |      |
|      |      | nce-action-t |                  |   |   |    |      |
|      |      | x-id]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  [\--governa |                  |   |   |    |      |
|      |      | nce-action-i |                  |   |   |    |      |
|      |      | ndex]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide an   |                  |   |   |    |      |
|      |      | anchor (url  |                  |   |   |    |      |
|      |      | / hash) of   |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | proposal. A  |                  |   |   |    |      |
|      |      | document     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | proposer     |                  |   |   |    |      |
|      |      | exposes the  |                  |   |   |    |      |
|      |      | reasoning    |                  |   |   |    |      |
|      |      | behind the   |                  |   |   |    |      |
|      |      | proposed     |                  |   |   |    |      |
|      |      | change.\     |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [\--anchor |                  |   |   |    |      |
|      |      | -url]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\--       |                  |   |   |    |      |
|      |      | anchor-data- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action (the  |                  |   |   |    |      |
|      |      | proposal)    |                  |   |   |    |      |
|      |      | will be      |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Detail Pending   |   |   |    |      |
|      |      | generated    |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action       |                  |   |   |    |      |
|      |      | complies     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl, |                  |   |   |    |      |
|      |      | wh           |                  |   |   |    |      |
|      |      | ere:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [propos      |                  |   |   |    |      |
|      |      | al_procedure |                  |   |   |    |      |
|      |      | =]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\[ deposit  |                  |   |   |    |      |
|      |      | :            |                  |   |   |    |      |
|      |      | coin]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | reward_acc   |                  |   |   |    |      |
|      |      | ount]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | gov_ac       |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | an           |                  |   |   |    |      |
|      |      | chor]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\]]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [n           |                  |   |   |    |      |
|      |      | o_confidence |                  |   |   |    |      |
|      |      | = (3,        |                  |   |   |    |      |
|      |      | g            |                  |   |   |    |      |
|      |      | ov_action_id |                  |   |   |    |      |
|      |      | /            |                  |   |   |    |      |
|      |      | n            |                  |   |   |    |      |
|      |      | ull)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [The command | Detail Pending   |   |   |    |      |
| LI19 | an   | requires     |                  |   |   |    |      |
|      | ada  | either       |                  |   |   |    |      |
|      | ho   | \--mainnet   |                  |   |   |    |      |
|      | lder | or           |                  |   |   |    |      |
|      |      | \--t         |                  |   |   |    |      |
|      | I    | estnet-magic |                  |   |   |    |      |
|      | want | NATURAL      |                  |   |   |    |      |
|      | to   | option to    |                  |   |   |    |      |
|      | cr   | specify the  |                  |   |   |    |      |
|      | eate | target       |                  |   |   |    |      |
|      | a    | network for  |                  |   |   |    |      |
|      | go   | which the    |                  |   |   |    |      |
|      | vern | action is    |                  |   |   |    |      |
|      | ance | genera       |                  |   |   |    |      |
|      | ac   | ted.]{.mark} |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | init |              |                  |   |   |    |      |
|      | iate |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | hard |              |                  |   |   |    |      |
|      | fork |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | s    |              |                  |   |   |    |      |
|      | ubmi |              |                  |   |   |    |      |
|      | tted |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | v    |              |                  |   |   |    |      |
|      | oted |              |                  |   |   |    |      |
|      | by   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | bo   |              |                  |   |   |    |      |
|      | dies |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | the deposit  |                  |   |   |    |      |
|      |      | amount for   |                  |   |   |    |      |
|      |      | submitting   |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | actions via  |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | mandatory    |                  |   |   |    |      |
|      |      | flag         |                  |   |   |    |      |
|      |      | *\           |                  |   |   |    |      |
|      |      | --governance |                  |   |   |    |      |
|      |      | -action-depo |                  |   |   |    |      |
|      |      | sit*]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | stake        |                  |   |   |    |      |
|      |      | credential   |                  |   |   |    |      |
|      |      | that will    |                  |   |   |    |      |
|      |      | receive the  |                  |   |   |    |      |
|      |      | deposit      |                  |   |   |    |      |
|      |      | return when  |                  |   |   |    |      |
|      |      | the action   |                  |   |   |    |      |
|      |      | is           |                  |   |   |    |      |
|      |      | enac         |                  |   |   |    |      |
|      |      | ted/expired. |                  |   |   |    |      |
|      |      | It accepts:\ |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [\-        |                  |   |   |    |      |
|      |      | -stake-verif |                  |   |   |    |      |
|      |      | ication-key- |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\--stake- |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | -key]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\         |                  |   |   |    |      |
|      |      | --stake-key- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | allows the   |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | transaction  |                  |   |   |    |      |
|      |      | id and index |                  |   |   |    |      |
|      |      | of the       |                  |   |   |    |      |
|      |      | previously   |                  |   |   |    |      |
|      |      | enacted      |                  |   |   |    |      |
|      |      | action of    |                  |   |   |    |      |
|      |      | this type.   |                  |   |   |    |      |
|      |      | These flags  |                  |   |   |    |      |
|      |      | are optional |                  |   |   |    |      |
|      |      | (but if one  |                  |   |   |    |      |
|      |      | is used the  |                  |   |   |    |      |
|      |      | other one    |                  |   |   |    |      |
|      |      | must be used |                  |   |   |    |      |
|      |      | too) to      |                  |   |   |    |      |
|      |      | support the  |                  |   |   |    |      |
|      |      | very first   |                  |   |   |    |      |
|      |      | action of    |                  |   |   |    |      |
|      |      | this type on |                  |   |   |    |      |
|      |      | the system   |                  |   |   |    |      |
|      |      | which does   |                  |   |   |    |      |
|      |      | not require  |                  |   |   |    |      |
|      |      | information  |                  |   |   |    |      |
|      |      | about        |                  |   |   |    |      |
|      |      | previously   |                  |   |   |    |      |
|      |      | enacted      |                  |   |   |    |      |
|      |      | actions. The |                  |   |   |    |      |
|      |      | flags        |                  |   |   |    |      |
|      |      | are:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  [\--governa |                  |   |   |    |      |
|      |      | nce-action-t |                  |   |   |    |      |
|      |      | x-id]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  [\--governa |                  |   |   |    |      |
|      |      | nce-action-i |                  |   |   |    |      |
|      |      | ndex]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide an   |                  |   |   |    |      |
|      |      | anchor (url  |                  |   |   |    |      |
|      |      | / hash) of   |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | proposal. A  |                  |   |   |    |      |
|      |      | document     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | proposer     |                  |   |   |    |      |
|      |      | exposes the  |                  |   |   |    |      |
|      |      | reasoning    |                  |   |   |    |      |
|      |      | behind the   |                  |   |   |    |      |
|      |      | proposed     |                  |   |   |    |      |
|      |      | change.\     |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [\--anchor |                  |   |   |    |      |
|      |      | -url]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\--       |                  |   |   |    |      |
|      |      | anchor-data- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | input the    |                  |   |   |    |      |
|      |      | new protocol |                  |   |   |    |      |
|      |      | version      |                  |   |   |    |      |
|      |      | nu           |                  |   |   |    |      |
|      |      | mber]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action (the  |                  |   |   |    |      |
|      |      | proposal)    |                  |   |   |    |      |
|      |      | will be      |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Detail Pending   |   |   |    |      |
|      |      | generated    |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action       |                  |   |   |    |      |
|      |      | complies     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl, |                  |   |   |    |      |
|      |      | wh           |                  |   |   |    |      |
|      |      | ere:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [propos      |                  |   |   |    |      |
|      |      | al_procedure |                  |   |   |    |      |
|      |      | =]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\[ deposit  |                  |   |   |    |      |
|      |      | :            |                  |   |   |    |      |
|      |      | coin]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | reward_acc   |                  |   |   |    |      |
|      |      | ount]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | gov_ac       |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | an           |                  |   |   |    |      |
|      |      | chor]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\]]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [har         |                  |   |   |    |      |
|      |      | d_fork_initi |                  |   |   |    |      |
|      |      | ation_action |                  |   |   |    |      |
|      |      | = (1,        |                  |   |   |    |      |
|      |      | g            |                  |   |   |    |      |
|      |      | ov_action_id |                  |   |   |    |      |
|      |      | / null,      |                  |   |   |    |      |
|      |      | \[pro        |                  |   |   |    |      |
|      |      | tocol_versio |                  |   |   |    |      |
|      |      | n\])]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [The command | Detail Pending   |   |   |    |      |
| LI20 | an   | takes an     |                  |   |   |    |      |
|      | ada  | action file  |                  |   |   |    |      |
|      | ho   | as           |                  |   |   |    |      |
|      | lder | i            |                  |   |   |    |      |
|      |      | nput]{.mark} |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | want |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | ins  |              |                  |   |   |    |      |
|      | pect |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | cont |              |                  |   |   |    |      |
|      | ents |              |                  |   |   |    |      |
|      | of a |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | ac   |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | file |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | ve   |              |                  |   |   |    |      |
|      | rify |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | is   |              |                  |   |   |    |      |
|      | cor  |              |                  |   |   |    |      |
|      | rect |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | fore |              |                  |   |   |    |      |
|      | su   |              |                  |   |   |    |      |
|      | bmit |              |                  |   |   |    |      |
|      | ting |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | in a |              |                  |   |   |    |      |
|      | tra  |              |                  |   |   |    |      |
|      | nsac |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | car  |              |                  |   |   |    |      |
|      | dano |              |                  |   |   |    |      |
|      | -cli |              |                  |   |   |    |      |
|      | co   |              |                  |   |   |    |      |
|      | nway |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | ac   |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | view |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Gives an    | Detail Pending   |   |   |    |      |
|      |      | option to    |                  |   |   |    |      |
|      |      | select the   |                  |   |   |    |      |
|      |      | output       |                  |   |   |    |      |
|      |      | format (json |                  |   |   |    |      |
|      |      | or           |                  |   |   |    |      |
|      |      | y            |                  |   |   |    |      |
|      |      | aml)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | output is    |                  |   |   |    |      |
|      |      | saved, if it |                  |   |   |    |      |
|      |      | is not       |                  |   |   |    |      |
|      |      | specified it |                  |   |   |    |      |
|      |      | is printed   |                  |   |   |    |      |
|      |      | to           |                  |   |   |    |      |
|      |      | st           |                  |   |   |    |      |
|      |      | dout]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The output  | Detail Pending   |   |   |    |      |
|      |      | shows the    |                  |   |   |    |      |
|      |      | information  |                  |   |   |    |      |
|      |      | of the       |                  |   |   |    |      |
|      |      | proposal     |                  |   |   |    |      |
|      |      | based on the |                  |   |   |    |      |
|      |      | proposal     |                  |   |   |    |      |
|      |      | procedures   |                  |   |   |    |      |
|      |      | on a human   |                  |   |   |    |      |
|      |      | readable     |                  |   |   |    |      |
|      |      | format:\     |                  |   |   |    |      |
|      |      | \            |                  |   |   |    |      |
|      |      | propos       |                  |   |   |    |      |
|      |      | al_procedure |                  |   |   |    |      |
|      |      | =]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\[ deposit  |                  |   |   |    |      |
|      |      | :            |                  |   |   |    |      |
|      |      | coin]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | reward_acc   |                  |   |   |    |      |
|      |      | ount]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | gov_ac       |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [,           |                  |   |   |    |      |
|      |      | an           |                  |   |   |    |      |
|      |      | chor]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\]]{.mark}  |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As a | [The command | Detail Pending   |   |   |    |      |
| LI21 | D    | provides a   |                  |   |   |    |      |
|      | rep, | way to       |                  |   |   |    |      |
|      | SPO  | vote]{.mark} |                  |   |   |    |      |
|      | or   |              |                  |   |   |    |      |
|      | CC   | > [          |                  |   |   |    |      |
|      | me   | yes,]{.mark} |                  |   |   |    |      |
|      | mber | >            |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      | I    |  [no]{.mark} |                  |   |   |    |      |
|      | want | >            |                  |   |   |    |      |
|      | to   | > [abs       |                  |   |   |    |      |
|      | cr   | tain]{.mark} |                  |   |   |    |      |
|      | eate |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | vote |              |                  |   |   |    |      |
|      | for  |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | ac   |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | inc  |              |                  |   |   |    |      |
|      | lude |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | in a |              |                  |   |   |    |      |
|      | tra  |              |                  |   |   |    |      |
|      | nsac |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | su   |              |                  |   |   |    |      |
|      | bmit |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | car  |              |                  |   |   |    |      |
|      | dano |              |                  |   |   |    |      |
|      | -cli |              |                  |   |   |    |      |
|      | co   |              |                  |   |   |    |      |
|      | nway |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | vote |              |                  |   |   |    |      |
|      | cr   |              |                  |   |   |    |      |
|      | eate |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Requires to | Detail Pending   |   |   |    |      |
|      |      | specify the  |                  |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action ID    |                  |   |   |    |      |
|      |      | and index    |                  |   |   |    |      |
|      |      | that the     |                  |   |   |    |      |
|      |      | vote is      |                  |   |   |    |      |
|      |      | ab           |                  |   |   |    |      |
|      |      | out.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Requires    | Detail Pending   |   |   |    |      |
|      |      | the user to  |                  |   |   |    |      |
|      |      | provide      |                  |   |   |    |      |
|      |      | DRep, SPO or |                  |   |   |    |      |
|      |      | CC           |                  |   |   |    |      |
|      |      | credent      |                  |   |   |    |      |
|      |      | ials]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | allows the   |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide an   |                  |   |   |    |      |
|      |      | optional     |                  |   |   |    |      |
|      |      | anchor (url  |                  |   |   |    |      |
|      |      | / hash) if   |                  |   |   |    |      |
|      |      | the user     |                  |   |   |    |      |
|      |      | wishes to    |                  |   |   |    |      |
|      |      | share the    |                  |   |   |    |      |
|      |      | reasoning    |                  |   |   |    |      |
|      |      | behind the   |                  |   |   |    |      |
|      |      | vote.\       |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [\--anchor |                  |   |   |    |      |
|      |      | -url]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [\--       |                  |   |   |    |      |
|      |      | anchor-data- |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | vote will be |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Detail Pending   |   |   |    |      |
|      |      | generated    |                  |   |   |    |      |
|      |      | vote         |                  |   |   |    |      |
|      |      | complies     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl  |                  |   |   |    |      |
|      |      | where\       |                  |   |   |    |      |
|      |      | \            |                  |   |   |    |      |
|      |      | votin        |                  |   |   |    |      |
|      |      | g_procedures |                  |   |   |    |      |
|      |      | = { + voter  |                  |   |   |    |      |
|      |      | =\> { +      |                  |   |   |    |      |
|      |      | g            |                  |   |   |    |      |
|      |      | ov_action_id |                  |   |   |    |      |
|      |      | =\>          |                  |   |   |    |      |
|      |      | voti         |                  |   |   |    |      |
|      |      | ng_procedure |                  |   |   |    |      |
|      |      | } }]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [voti        |                  |   |   |    |      |
|      |      | ng_procedure |                  |   |   |    |      |
|      |      | =]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\[          |                  |   |   |    |      |
|      |      | vote]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, anchor /  |                  |   |   |    |      |
|      |      | null]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\]]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [; no -      |                  |   |   |    |      |
|      |      | 0]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [; yes -     |                  |   |   |    |      |
|      |      | 1]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [; abstain - |                  |   |   |    |      |
|      |      | 2]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [vote = 0 .. |                  |   |   |    |      |
|      |      | 2]{.mark}    |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As a | [The command | Detail Pending   |   |   |    |      |
| LI22 | D    | takes a vote |                  |   |   |    |      |
|      | Rep, | file as an   |                  |   |   |    |      |
|      | SPO  | i            |                  |   |   |    |      |
|      | or   | nput]{.mark} |                  |   |   |    |      |
|      | CC   |              |                  |   |   |    |      |
|      | me   |              |                  |   |   |    |      |
|      | mber |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | want |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | ins  |              |                  |   |   |    |      |
|      | pect |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | cont |              |                  |   |   |    |      |
|      | ents |              |                  |   |   |    |      |
|      | of a |              |                  |   |   |    |      |
|      | vote |              |                  |   |   |    |      |
|      | file |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | ve   |              |                  |   |   |    |      |
|      | rify |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | is   |              |                  |   |   |    |      |
|      | cor  |              |                  |   |   |    |      |
|      | rect |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | fore |              |                  |   |   |    |      |
|      | su   |              |                  |   |   |    |      |
|      | bmit |              |                  |   |   |    |      |
|      | ting |              |                  |   |   |    |      |
|      | it   |              |                  |   |   |    |      |
|      | in a |              |                  |   |   |    |      |
|      | tra  |              |                  |   |   |    |      |
|      | nsac |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | car  |              |                  |   |   |    |      |
|      | dano |              |                  |   |   |    |      |
|      | -cli |              |                  |   |   |    |      |
|      | co   |              |                  |   |   |    |      |
|      | nway |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | vote |              |                  |   |   |    |      |
|      | view |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Gives an    | Detail Pending   |   |   |    |      |
|      |      | option to    |                  |   |   |    |      |
|      |      | select the   |                  |   |   |    |      |
|      |      | output       |                  |   |   |    |      |
|      |      | format (json |                  |   |   |    |      |
|      |      | or           |                  |   |   |    |      |
|      |      | y            |                  |   |   |    |      |
|      |      | aml)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | output is    |                  |   |   |    |      |
|      |      | saved, if it |                  |   |   |    |      |
|      |      | is not       |                  |   |   |    |      |
|      |      | specified it |                  |   |   |    |      |
|      |      | is printed   |                  |   |   |    |      |
|      |      | to           |                  |   |   |    |      |
|      |      | st           |                  |   |   |    |      |
|      |      | dout]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The output  | Detail Pending   |   |   |    |      |
|      |      | shows the    |                  |   |   |    |      |
|      |      | information  |                  |   |   |    |      |
|      |      | of the       |                  |   |   |    |      |
|      |      | proposal     |                  |   |   |    |      |
|      |      | based on the |                  |   |   |    |      |
|      |      | voting       |                  |   |   |    |      |
|      |      | procedures   |                  |   |   |    |      |
|      |      | in a human   |                  |   |   |    |      |
|      |      | readable     |                  |   |   |    |      |
|      |      | format       |                  |   |   |    |      |
|      |      | (engli       |                  |   |   |    |      |
|      |      | sh):]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [votin       |                  |   |   |    |      |
|      |      | g_procedures |                  |   |   |    |      |
|      |      | = { + voter  |                  |   |   |    |      |
|      |      | =\> { +      |                  |   |   |    |      |
|      |      | g            |                  |   |   |    |      |
|      |      | ov_action_id |                  |   |   |    |      |
|      |      | =\>          |                  |   |   |    |      |
|      |      | voti         |                  |   |   |    |      |
|      |      | ng_procedure |                  |   |   |    |      |
|      |      | } }]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [voti        |                  |   |   |    |      |
|      |      | ng_procedure |                  |   |   |    |      |
|      |      | =]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\[          |                  |   |   |    |      |
|      |      | vote]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, anchor /  |                  |   |   |    |      |
|      |      | null]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\]]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [; no -      |                  |   |   |    |      |
|      |      | 0]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [; yes -     |                  |   |   |    |      |
|      |      | 1]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [; abstain - |                  |   |   |    |      |
|      |      | 2]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [vote = 0 .. |                  |   |   |    |      |
|      |      | 2]{.mark}    |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [Transaction | Detail Pending   |   |   |    |      |
| LI23 | an   | build has a  |                  |   |   |    |      |
|      | ada  | new flag to  |                  |   |   |    |      |
|      | ho   | supply a     |                  |   |   |    |      |
|      | lder | proposal     |                  |   |   |    |      |
|      |      | file as      |                  |   |   |    |      |
|      | I    | input for    |                  |   |   |    |      |
|      | want | the          |                  |   |   |    |      |
|      | to   | transaction  |                  |   |   |    |      |
|      | b    | body]{.mark} |                  |   |   |    |      |
|      | uild |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | tra  |              |                  |   |   |    |      |
|      | nsac |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | incl |              |                  |   |   |    |      |
|      | udes |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | prop |              |                  |   |   |    |      |
|      | osal |              |                  |   |   |    |      |
|      | (co  |              |                  |   |   |    |      |
|      | ntai |              |                  |   |   |    |      |
|      | ning |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | act  |              |                  |   |   |    |      |
|      | ion) |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | l    |              |                  |   |   |    |      |
|      | ater |              |                  |   |   |    |      |
|      | sign |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | su   |              |                  |   |   |    |      |
|      | bmit |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | tra  |              |                  |   |   |    |      |
|      | nsac |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | b    |              |                  |   |   |    |      |
|      | uild |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [When        | Detail Pending   |   |   |    |      |
|      |      | constructing |                  |   |   |    |      |
|      |      | a            |                  |   |   |    |      |
|      |      | transaction  |                  |   |   |    |      |
|      |      | body that    |                  |   |   |    |      |
|      |      | includes a   |                  |   |   |    |      |
|      |      | proposal,    |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | resulting tx |                  |   |   |    |      |
|      |      | body         |                  |   |   |    |      |
|      |      | conforms to  |                  |   |   |    |      |
|      |      | the conway   |                  |   |   |    |      |
|      |      | cddl so that |                  |   |   |    |      |
|      |      | proposal     |                  |   |   |    |      |
|      |      | procedures   |                  |   |   |    |      |
|      |      | are recorded |                  |   |   |    |      |
|      |      | with the key |                  |   |   |    |      |
|      |      | 20\          |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [tran        |                  |   |   |    |      |
|      |      | saction_body |                  |   |   |    |      |
|      |      | =]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [{ 0 :       |                  |   |   |    |      |
|      |      | set\<transac |                  |   |   |    |      |
|      |      | tion_input\> |                  |   |   |    |      |
|      |      | ;            |                  |   |   |    |      |
|      |      | in           |                  |   |   |    |      |
|      |      | puts]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, 1 : \[\*  |                  |   |   |    |      |
|      |      | tran         |                  |   |   |    |      |
|      |      | saction_outp |                  |   |   |    |      |
|      |      | ut\]]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, 2 : coin  |                  |   |   |    |      |
|      |      | ;            |                  |   |   |    |      |
|      |      | fee]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 3 :     |                  |   |   |    |      |
|      |      | uint ; time  |                  |   |   |    |      |
|      |      | to           |                  |   |   |    |      |
|      |      | live]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 4 :     |                  |   |   |    |      |
|      |      | certific     |                  |   |   |    |      |
|      |      | ates]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 5 :     |                  |   |   |    |      |
|      |      | withdra      |                  |   |   |    |      |
|      |      | wals]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 7 :     |                  |   |   |    |      |
|      |      | aux          |                  |   |   |    |      |
|      |      | iliary_data_ |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 8 :     |                  |   |   |    |      |
|      |      | uint ;       |                  |   |   |    |      |
|      |      | validity     |                  |   |   |    |      |
|      |      | interval     |                  |   |   |    |      |
|      |      | s            |                  |   |   |    |      |
|      |      | tart]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 9 :     |                  |   |   |    |      |
|      |      | mint]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 11 :    |                  |   |   |    |      |
|      |      | script_data_ |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 13 :    |                  |   |   |    |      |
|      |      | nonempty_    |                  |   |   |    |      |
|      |      | set\<transac |                  |   |   |    |      |
|      |      | tion_input\> |                  |   |   |    |      |
|      |      | ; collateral |                  |   |   |    |      |
|      |      | in           |                  |   |   |    |      |
|      |      | puts]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 14 :    |                  |   |   |    |      |
|      |      | required_sig |                  |   |   |    |      |
|      |      | ners]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 15 :    |                  |   |   |    |      |
|      |      | networ       |                  |   |   |    |      |
|      |      | k_id]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 16 :    |                  |   |   |    |      |
|      |      | transa       |                  |   |   |    |      |
|      |      | ction_output |                  |   |   |    |      |
|      |      | ; collateral |                  |   |   |    |      |
|      |      | re           |                  |   |   |    |      |
|      |      | turn]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 17 :    |                  |   |   |    |      |
|      |      | coin ; total |                  |   |   |    |      |
|      |      | collat       |                  |   |   |    |      |
|      |      | eral]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 18 :    |                  |   |   |    |      |
|      |      | nonempty_    |                  |   |   |    |      |
|      |      | set\<transac |                  |   |   |    |      |
|      |      | tion_input\> |                  |   |   |    |      |
|      |      | ; reference  |                  |   |   |    |      |
|      |      | in           |                  |   |   |    |      |
|      |      | puts]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 19 :    |                  |   |   |    |      |
|      |      | votin        |                  |   |   |    |      |
|      |      | g_procedures |                  |   |   |    |      |
|      |      | ; New;       |                  |   |   |    |      |
|      |      | Voting       |                  |   |   |    |      |
|      |      | proced       |                  |   |   |    |      |
|      |      | ures]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 20 :    |                  |   |   |    |      |
|      |      | proposa      |                  |   |   |    |      |
|      |      | l_procedures |                  |   |   |    |      |
|      |      | ; New;       |                  |   |   |    |      |
|      |      | Proposal     |                  |   |   |    |      |
|      |      | proced       |                  |   |   |    |      |
|      |      | ures]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 21 :    |                  |   |   |    |      |
|      |      | coin ; New;  |                  |   |   |    |      |
|      |      | current      |                  |   |   |    |      |
|      |      | treasury     |                  |   |   |    |      |
|      |      | v            |                  |   |   |    |      |
|      |      | alue]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 22 :    |                  |   |   |    |      |
|      |      | p            |                  |   |   |    |      |
|      |      | ositive_coin |                  |   |   |    |      |
|      |      | ; New;       |                  |   |   |    |      |
|      |      | dona         |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [}]{.mark}   |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As a | [Transaction | Detail Pending   |   |   |    |      |
| LI24 | D    | build has a  |                  |   |   |    |      |
|      | Rep, | new flag to  |                  |   |   |    |      |
|      | SPO  | supply a     |                  |   |   |    |      |
|      | or   | vote file as |                  |   |   |    |      |
|      | CC   | input for    |                  |   |   |    |      |
|      | me   | the          |                  |   |   |    |      |
|      | mber | transaction  |                  |   |   |    |      |
|      |      | body]{.mark} |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | want |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | b    |              |                  |   |   |    |      |
|      | uild |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | tra  |              |                  |   |   |    |      |
|      | nsac |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | incl |              |                  |   |   |    |      |
|      | udes |              |                  |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | vote |              |                  |   |   |    |      |
|      | on a |              |                  |   |   |    |      |
|      | pa   |              |                  |   |   |    |      |
|      | rtic |              |                  |   |   |    |      |
|      | ular |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | ac   |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | l    |              |                  |   |   |    |      |
|      | ater |              |                  |   |   |    |      |
|      | sign |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | su   |              |                  |   |   |    |      |
|      | bmit |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | tra  |              |                  |   |   |    |      |
|      | nsac |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | b    |              |                  |   |   |    |      |
|      | uild |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [When        | Detail Pending   |   |   |    |      |
|      |      | constructing |                  |   |   |    |      |
|      |      | a            |                  |   |   |    |      |
|      |      | transaction  |                  |   |   |    |      |
|      |      | body that    |                  |   |   |    |      |
|      |      | includes a   |                  |   |   |    |      |
|      |      | vote, the    |                  |   |   |    |      |
|      |      | resulting tx |                  |   |   |    |      |
|      |      | body         |                  |   |   |    |      |
|      |      | conforms to  |                  |   |   |    |      |
|      |      | the conway   |                  |   |   |    |      |
|      |      | cddl so that |                  |   |   |    |      |
|      |      | voting       |                  |   |   |    |      |
|      |      | procedures   |                  |   |   |    |      |
|      |      | are recorded |                  |   |   |    |      |
|      |      | with the key |                  |   |   |    |      |
|      |      | 19\          |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [tran        |                  |   |   |    |      |
|      |      | saction_body |                  |   |   |    |      |
|      |      | =]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [{ 0 :       |                  |   |   |    |      |
|      |      | set\<transac |                  |   |   |    |      |
|      |      | tion_input\> |                  |   |   |    |      |
|      |      | ;            |                  |   |   |    |      |
|      |      | in           |                  |   |   |    |      |
|      |      | puts]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, 1 : \[\*  |                  |   |   |    |      |
|      |      | tran         |                  |   |   |    |      |
|      |      | saction_outp |                  |   |   |    |      |
|      |      | ut\]]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, 2 : coin  |                  |   |   |    |      |
|      |      | ;            |                  |   |   |    |      |
|      |      | fee]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 3 :     |                  |   |   |    |      |
|      |      | uint ; time  |                  |   |   |    |      |
|      |      | to           |                  |   |   |    |      |
|      |      | live]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 4 :     |                  |   |   |    |      |
|      |      | certific     |                  |   |   |    |      |
|      |      | ates]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 5 :     |                  |   |   |    |      |
|      |      | withdra      |                  |   |   |    |      |
|      |      | wals]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 7 :     |                  |   |   |    |      |
|      |      | aux          |                  |   |   |    |      |
|      |      | iliary_data_ |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 8 :     |                  |   |   |    |      |
|      |      | uint ;       |                  |   |   |    |      |
|      |      | validity     |                  |   |   |    |      |
|      |      | interval     |                  |   |   |    |      |
|      |      | s            |                  |   |   |    |      |
|      |      | tart]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 9 :     |                  |   |   |    |      |
|      |      | mint]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 11 :    |                  |   |   |    |      |
|      |      | script_data_ |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 13 :    |                  |   |   |    |      |
|      |      | nonempty_    |                  |   |   |    |      |
|      |      | set\<transac |                  |   |   |    |      |
|      |      | tion_input\> |                  |   |   |    |      |
|      |      | ; collateral |                  |   |   |    |      |
|      |      | in           |                  |   |   |    |      |
|      |      | puts]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 14 :    |                  |   |   |    |      |
|      |      | required_sig |                  |   |   |    |      |
|      |      | ners]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 15 :    |                  |   |   |    |      |
|      |      | networ       |                  |   |   |    |      |
|      |      | k_id]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 16 :    |                  |   |   |    |      |
|      |      | transa       |                  |   |   |    |      |
|      |      | ction_output |                  |   |   |    |      |
|      |      | ; collateral |                  |   |   |    |      |
|      |      | re           |                  |   |   |    |      |
|      |      | turn]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 17 :    |                  |   |   |    |      |
|      |      | coin ; total |                  |   |   |    |      |
|      |      | collat       |                  |   |   |    |      |
|      |      | eral]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 18 :    |                  |   |   |    |      |
|      |      | nonempty_    |                  |   |   |    |      |
|      |      | set\<transac |                  |   |   |    |      |
|      |      | tion_input\> |                  |   |   |    |      |
|      |      | ; reference  |                  |   |   |    |      |
|      |      | in           |                  |   |   |    |      |
|      |      | puts]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 19 :    |                  |   |   |    |      |
|      |      | votin        |                  |   |   |    |      |
|      |      | g_procedures |                  |   |   |    |      |
|      |      | ; New;       |                  |   |   |    |      |
|      |      | Voting       |                  |   |   |    |      |
|      |      | proced       |                  |   |   |    |      |
|      |      | ures]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 20 :    |                  |   |   |    |      |
|      |      | proposa      |                  |   |   |    |      |
|      |      | l_procedures |                  |   |   |    |      |
|      |      | ; New;       |                  |   |   |    |      |
|      |      | Proposal     |                  |   |   |    |      |
|      |      | proced       |                  |   |   |    |      |
|      |      | ures]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 21 :    |                  |   |   |    |      |
|      |      | coin ; New;  |                  |   |   |    |      |
|      |      | current      |                  |   |   |    |      |
|      |      | treasury     |                  |   |   |    |      |
|      |      | v            |                  |   |   |    |      |
|      |      | alue]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 22 :    |                  |   |   |    |      |
|      |      | p            |                  |   |   |    |      |
|      |      | ositive_coin |                  |   |   |    |      |
|      |      | ; New;       |                  |   |   |    |      |
|      |      | dona         |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [}]{.mark}   |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [Transaction | Detail Pending   |   |   |    |      |
| LI25 | an   | build-raw    |                  |   |   |    |      |
|      | ada  | has a new    |                  |   |   |    |      |
|      | ho   | flag to      |                  |   |   |    |      |
|      | lder | supply a     |                  |   |   |    |      |
|      |      | proposal     |                  |   |   |    |      |
|      | I    | file as      |                  |   |   |    |      |
|      | want | input for    |                  |   |   |    |      |
|      | to   | the          |                  |   |   |    |      |
|      | b    | transaction  |                  |   |   |    |      |
|      | uild | body]{.mark} |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | tra  |              |                  |   |   |    |      |
|      | nsac |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | incl |              |                  |   |   |    |      |
|      | udes |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | prop |              |                  |   |   |    |      |
|      | osal |              |                  |   |   |    |      |
|      | (co  |              |                  |   |   |    |      |
|      | ntai |              |                  |   |   |    |      |
|      | ning |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | act  |              |                  |   |   |    |      |
|      | ion) |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | l    |              |                  |   |   |    |      |
|      | ater |              |                  |   |   |    |      |
|      | sign |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | su   |              |                  |   |   |    |      |
|      | bmit |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | tra  |              |                  |   |   |    |      |
|      | nsac |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | b    |              |                  |   |   |    |      |
|      | uild |              |                  |   |   |    |      |
|      | -raw |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [When        | Detail Pending   |   |   |    |      |
|      |      | constructing |                  |   |   |    |      |
|      |      | a            |                  |   |   |    |      |
|      |      | transaction  |                  |   |   |    |      |
|      |      | body that    |                  |   |   |    |      |
|      |      | includes a   |                  |   |   |    |      |
|      |      | proposal,    |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      |      | resulting tx |                  |   |   |    |      |
|      |      | body         |                  |   |   |    |      |
|      |      | conforms to  |                  |   |   |    |      |
|      |      | the conway   |                  |   |   |    |      |
|      |      | cddl so that |                  |   |   |    |      |
|      |      | proposal     |                  |   |   |    |      |
|      |      | procedures   |                  |   |   |    |      |
|      |      | are recorded |                  |   |   |    |      |
|      |      | with the key |                  |   |   |    |      |
|      |      | 20\          |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [tran        |                  |   |   |    |      |
|      |      | saction_body |                  |   |   |    |      |
|      |      | =]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [{ 0 :       |                  |   |   |    |      |
|      |      | set\<transac |                  |   |   |    |      |
|      |      | tion_input\> |                  |   |   |    |      |
|      |      | ;            |                  |   |   |    |      |
|      |      | in           |                  |   |   |    |      |
|      |      | puts]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, 1 : \[\*  |                  |   |   |    |      |
|      |      | tran         |                  |   |   |    |      |
|      |      | saction_outp |                  |   |   |    |      |
|      |      | ut\]]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, 2 : coin  |                  |   |   |    |      |
|      |      | ;            |                  |   |   |    |      |
|      |      | fee]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 3 :     |                  |   |   |    |      |
|      |      | uint ; time  |                  |   |   |    |      |
|      |      | to           |                  |   |   |    |      |
|      |      | live]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 4 :     |                  |   |   |    |      |
|      |      | certific     |                  |   |   |    |      |
|      |      | ates]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 5 :     |                  |   |   |    |      |
|      |      | withdra      |                  |   |   |    |      |
|      |      | wals]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 7 :     |                  |   |   |    |      |
|      |      | aux          |                  |   |   |    |      |
|      |      | iliary_data_ |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 8 :     |                  |   |   |    |      |
|      |      | uint ;       |                  |   |   |    |      |
|      |      | validity     |                  |   |   |    |      |
|      |      | interval     |                  |   |   |    |      |
|      |      | s            |                  |   |   |    |      |
|      |      | tart]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 9 :     |                  |   |   |    |      |
|      |      | mint]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 11 :    |                  |   |   |    |      |
|      |      | script_data_ |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 13 :    |                  |   |   |    |      |
|      |      | nonempty_    |                  |   |   |    |      |
|      |      | set\<transac |                  |   |   |    |      |
|      |      | tion_input\> |                  |   |   |    |      |
|      |      | ; collateral |                  |   |   |    |      |
|      |      | in           |                  |   |   |    |      |
|      |      | puts]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 14 :    |                  |   |   |    |      |
|      |      | required_sig |                  |   |   |    |      |
|      |      | ners]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 15 :    |                  |   |   |    |      |
|      |      | networ       |                  |   |   |    |      |
|      |      | k_id]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 16 :    |                  |   |   |    |      |
|      |      | transa       |                  |   |   |    |      |
|      |      | ction_output |                  |   |   |    |      |
|      |      | ; collateral |                  |   |   |    |      |
|      |      | re           |                  |   |   |    |      |
|      |      | turn]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 17 :    |                  |   |   |    |      |
|      |      | coin ; total |                  |   |   |    |      |
|      |      | collat       |                  |   |   |    |      |
|      |      | eral]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 18 :    |                  |   |   |    |      |
|      |      | nonempty_    |                  |   |   |    |      |
|      |      | set\<transac |                  |   |   |    |      |
|      |      | tion_input\> |                  |   |   |    |      |
|      |      | ; reference  |                  |   |   |    |      |
|      |      | in           |                  |   |   |    |      |
|      |      | puts]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 19 :    |                  |   |   |    |      |
|      |      | votin        |                  |   |   |    |      |
|      |      | g_procedures |                  |   |   |    |      |
|      |      | ; New;       |                  |   |   |    |      |
|      |      | Voting       |                  |   |   |    |      |
|      |      | proced       |                  |   |   |    |      |
|      |      | ures]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 20 :    |                  |   |   |    |      |
|      |      | proposa      |                  |   |   |    |      |
|      |      | l_procedures |                  |   |   |    |      |
|      |      | ; New;       |                  |   |   |    |      |
|      |      | Proposal     |                  |   |   |    |      |
|      |      | proced       |                  |   |   |    |      |
|      |      | ures]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 21 :    |                  |   |   |    |      |
|      |      | coin ; New;  |                  |   |   |    |      |
|      |      | current      |                  |   |   |    |      |
|      |      | treasury     |                  |   |   |    |      |
|      |      | v            |                  |   |   |    |      |
|      |      | alue]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 22 :    |                  |   |   |    |      |
|      |      | p            |                  |   |   |    |      |
|      |      | ositive_coin |                  |   |   |    |      |
|      |      | ; New;       |                  |   |   |    |      |
|      |      | dona         |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [}]{.mark}   |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As a | [Transaction | Detail Pending   |   |   |    |      |
| LI26 | D    | build-raw    |                  |   |   |    |      |
|      | Rep, | has a new    |                  |   |   |    |      |
|      | SPO  | flag to      |                  |   |   |    |      |
|      | or   | supply a     |                  |   |   |    |      |
|      | CC   | vote file as |                  |   |   |    |      |
|      | me   | input for    |                  |   |   |    |      |
|      | mber | the          |                  |   |   |    |      |
|      |      | transaction  |                  |   |   |    |      |
|      | I    | body]{.mark} |                  |   |   |    |      |
|      | want |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | b    |              |                  |   |   |    |      |
|      | uild |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | tra  |              |                  |   |   |    |      |
|      | nsac |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | incl |              |                  |   |   |    |      |
|      | udes |              |                  |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | vote |              |                  |   |   |    |      |
|      | on a |              |                  |   |   |    |      |
|      | pa   |              |                  |   |   |    |      |
|      | rtic |              |                  |   |   |    |      |
|      | ular |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | ac   |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | l    |              |                  |   |   |    |      |
|      | ater |              |                  |   |   |    |      |
|      | sign |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | su   |              |                  |   |   |    |      |
|      | bmit |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | tra  |              |                  |   |   |    |      |
|      | nsac |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | b    |              |                  |   |   |    |      |
|      | uild |              |                  |   |   |    |      |
|      | -raw |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [When        | Detail Pending   |   |   |    |      |
|      |      | constructing |                  |   |   |    |      |
|      |      | a            |                  |   |   |    |      |
|      |      | transaction  |                  |   |   |    |      |
|      |      | body that    |                  |   |   |    |      |
|      |      | includes a   |                  |   |   |    |      |
|      |      | vote, the    |                  |   |   |    |      |
|      |      | resulting tx |                  |   |   |    |      |
|      |      | body         |                  |   |   |    |      |
|      |      | conforms to  |                  |   |   |    |      |
|      |      | the conway   |                  |   |   |    |      |
|      |      | cddl so that |                  |   |   |    |      |
|      |      | voting       |                  |   |   |    |      |
|      |      | procedures   |                  |   |   |    |      |
|      |      | are recorded |                  |   |   |    |      |
|      |      | with the key |                  |   |   |    |      |
|      |      | 19\          |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [tran        |                  |   |   |    |      |
|      |      | saction_body |                  |   |   |    |      |
|      |      | =]{.mark}    |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [{ 0 :       |                  |   |   |    |      |
|      |      | set\<transac |                  |   |   |    |      |
|      |      | tion_input\> |                  |   |   |    |      |
|      |      | ;            |                  |   |   |    |      |
|      |      | in           |                  |   |   |    |      |
|      |      | puts]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, 1 : \[\*  |                  |   |   |    |      |
|      |      | tran         |                  |   |   |    |      |
|      |      | saction_outp |                  |   |   |    |      |
|      |      | ut\]]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, 2 : coin  |                  |   |   |    |      |
|      |      | ;            |                  |   |   |    |      |
|      |      | fee]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 3 :     |                  |   |   |    |      |
|      |      | uint ; time  |                  |   |   |    |      |
|      |      | to           |                  |   |   |    |      |
|      |      | live]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 4 :     |                  |   |   |    |      |
|      |      | certific     |                  |   |   |    |      |
|      |      | ates]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 5 :     |                  |   |   |    |      |
|      |      | withdra      |                  |   |   |    |      |
|      |      | wals]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 7 :     |                  |   |   |    |      |
|      |      | aux          |                  |   |   |    |      |
|      |      | iliary_data_ |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 8 :     |                  |   |   |    |      |
|      |      | uint ;       |                  |   |   |    |      |
|      |      | validity     |                  |   |   |    |      |
|      |      | interval     |                  |   |   |    |      |
|      |      | s            |                  |   |   |    |      |
|      |      | tart]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 9 :     |                  |   |   |    |      |
|      |      | mint]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 11 :    |                  |   |   |    |      |
|      |      | script_data_ |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 13 :    |                  |   |   |    |      |
|      |      | nonempty_    |                  |   |   |    |      |
|      |      | set\<transac |                  |   |   |    |      |
|      |      | tion_input\> |                  |   |   |    |      |
|      |      | ; collateral |                  |   |   |    |      |
|      |      | in           |                  |   |   |    |      |
|      |      | puts]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 14 :    |                  |   |   |    |      |
|      |      | required_sig |                  |   |   |    |      |
|      |      | ners]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 15 :    |                  |   |   |    |      |
|      |      | networ       |                  |   |   |    |      |
|      |      | k_id]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 16 :    |                  |   |   |    |      |
|      |      | transa       |                  |   |   |    |      |
|      |      | ction_output |                  |   |   |    |      |
|      |      | ; collateral |                  |   |   |    |      |
|      |      | re           |                  |   |   |    |      |
|      |      | turn]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 17 :    |                  |   |   |    |      |
|      |      | coin ; total |                  |   |   |    |      |
|      |      | collat       |                  |   |   |    |      |
|      |      | eral]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 18 :    |                  |   |   |    |      |
|      |      | nonempty_    |                  |   |   |    |      |
|      |      | set\<transac |                  |   |   |    |      |
|      |      | tion_input\> |                  |   |   |    |      |
|      |      | ; reference  |                  |   |   |    |      |
|      |      | in           |                  |   |   |    |      |
|      |      | puts]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 19 :    |                  |   |   |    |      |
|      |      | votin        |                  |   |   |    |      |
|      |      | g_procedures |                  |   |   |    |      |
|      |      | ; New;       |                  |   |   |    |      |
|      |      | Voting       |                  |   |   |    |      |
|      |      | proced       |                  |   |   |    |      |
|      |      | ures]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 20 :    |                  |   |   |    |      |
|      |      | proposa      |                  |   |   |    |      |
|      |      | l_procedures |                  |   |   |    |      |
|      |      | ; New;       |                  |   |   |    |      |
|      |      | Proposal     |                  |   |   |    |      |
|      |      | proced       |                  |   |   |    |      |
|      |      | ures]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 21 :    |                  |   |   |    |      |
|      |      | coin ; New;  |                  |   |   |    |      |
|      |      | current      |                  |   |   |    |      |
|      |      | treasury     |                  |   |   |    |      |
|      |      | v            |                  |   |   |    |      |
|      |      | alue]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [, ? 22 :    |                  |   |   |    |      |
|      |      | p            |                  |   |   |    |      |
|      |      | ositive_coin |                  |   |   |    |      |
|      |      | ; New;       |                  |   |   |    |      |
|      |      | dona         |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [}]{.mark}   |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [Allows the  | Detail Pending   |   |   |    |      |
| LI27 | an   | user to      |                  |   |   |    |      |
|      | ada  | provide      |                  |   |   |    |      |
|      | ho   | credentials  |                  |   |   |    |      |
|      | lder | in any of    |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      | I    | following    |                  |   |   |    |      |
|      | want | fo           |                  |   |   |    |      |
|      | to   | rms:]{.mark} |                  |   |   |    |      |
|      | cr   |              |                  |   |   |    |      |
|      | eate | > [Stake     |                  |   |   |    |      |
|      | a    | >            |                  |   |   |    |      |
|      | co   | verification |                  |   |   |    |      |
|      | nway | >            |                  |   |   |    |      |
|      | cd   |  key]{.mark} |                  |   |   |    |      |
|      | dl-c | >            |                  |   |   |    |      |
|      | ompl | > [Stake     |                  |   |   |    |      |
|      | iant | >            |                  |   |   |    |      |
|      | s    | verification |                  |   |   |    |      |
|      | take | > key        |                  |   |   |    |      |
|      | regi | >            |                  |   |   |    |      |
|      | stra | file]{.mark} |                  |   |   |    |      |
|      | tion | >            |                  |   |   |    |      |
|      | cer  | > [Stake     |                  |   |   |    |      |
|      | tifi | > add        |                  |   |   |    |      |
|      | cate | ress]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      | s    | > [Stake     |                  |   |   |    |      |
|      | take | > script     |                  |   |   |    |      |
|      | -add | >            |                  |   |   |    |      |
|      | ress | file]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Requires    | Detail Pending   |   |   |    |      |
|      |      | the user to  |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | required key |                  |   |   |    |      |
|      |      | deposit in   |                  |   |   |    |      |
|      |      | love         |                  |   |   |    |      |
|      |      | lace]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | registration |                  |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | will be      |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | handles      |                  |   |   |    |      |
|      |      | errors       |                  |   |   |    |      |
|      |      | gracefully   |                  |   |   |    |      |
|      |      | and provides |                  |   |   |    |      |
|      |      | helpful      |                  |   |   |    |      |
|      |      | error        |                  |   |   |    |      |
|      |      | messages     |                  |   |   |    |      |
|      |      | when         |                  |   |   |    |      |
|      |      | required     |                  |   |   |    |      |
|      |      | options are  |                  |   |   |    |      |
|      |      | missing or   |                  |   |   |    |      |
|      |      | invalid      |                  |   |   |    |      |
|      |      | inputs are   |                  |   |   |    |      |
|      |      | provi        |                  |   |   |    |      |
|      |      | ded.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Detail Pending   |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | should be    |                  |   |   |    |      |
|      |      | saved on a   |                  |   |   |    |      |
|      |      | text         |                  |   |   |    |      |
|      |      | envelope     |                  |   |   |    |      |
|      |      | for          |                  |   |   |    |      |
|      |      | mat:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [{]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\"type\":   |                  |   |   |    |      |
|      |      | \"Cert       |                  |   |   |    |      |
|      |      | ificateConwa |                  |   |   |    |      |
|      |      | y\",]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\"de        |                  |   |   |    |      |
|      |      | scription\": |                  |   |   |    |      |
|      |      | \"Stake      |                  |   |   |    |      |
|      |      | Address      |                  |   |   |    |      |
|      |      | Registration |                  |   |   |    |      |
|      |      | Certificat   |                  |   |   |    |      |
|      |      | e\",]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [            |                  |   |   |    |      |
|      |      | \"cborHex\": |                  |   |   |    |      |
|      |      | \"\"]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [}]{.mark}   |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | []{.mark}   |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Detail Pending   |   |   |    |      |
|      |      | resulting    |                  |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | conforms     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl, |                  |   |   |    |      |
|      |      | where\       |                  |   |   |    |      |
|      |      | \            |                  |   |   |    |      |
|      |      | reg_cert =   |                  |   |   |    |      |
|      |      | (7,          |                  |   |   |    |      |
|      |      | stake        |                  |   |   |    |      |
|      |      | _credential, |                  |   |   |    |      |
|      |      | c            |                  |   |   |    |      |
|      |      | oin)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [Allows the  | Detail Pending   |   |   |    |      |
| LI28 | an   | user to      |                  |   |   |    |      |
|      | ada  | provide      |                  |   |   |    |      |
|      | ho   | credentials  |                  |   |   |    |      |
|      | lder | in any of    |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      | I    | following    |                  |   |   |    |      |
|      | want | fo           |                  |   |   |    |      |
|      | to   | rms:]{.mark} |                  |   |   |    |      |
|      | cr   |              |                  |   |   |    |      |
|      | eate | > [Stake     |                  |   |   |    |      |
|      | a    | >            |                  |   |   |    |      |
|      | co   | verification |                  |   |   |    |      |
|      | nway | >            |                  |   |   |    |      |
|      | cd   |  key]{.mark} |                  |   |   |    |      |
|      | dl-c | >            |                  |   |   |    |      |
|      | ompl | > [Stake     |                  |   |   |    |      |
|      | iant | >            |                  |   |   |    |      |
|      | s    | verification |                  |   |   |    |      |
|      | take | > key        |                  |   |   |    |      |
|      | de   | >            |                  |   |   |    |      |
|      | regi | file]{.mark} |                  |   |   |    |      |
|      | stra | >            |                  |   |   |    |      |
|      | tion | > [Stake     |                  |   |   |    |      |
|      | cer  | > add        |                  |   |   |    |      |
|      | tifi | ress]{.mark} |                  |   |   |    |      |
|      | cate | >            |                  |   |   |    |      |
|      | to   | > [Stake     |                  |   |   |    |      |
|      | get  | > script     |                  |   |   |    |      |
|      | my   | >            |                  |   |   |    |      |
|      | dep  | file]{.mark} |                  |   |   |    |      |
|      | osit |              |                  |   |   |    |      |
|      | back |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | s    |              |                  |   |   |    |      |
|      | take |              |                  |   |   |    |      |
|      | -add |              |                  |   |   |    |      |
|      | ress |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Requires    | Detail Pending   |   |   |    |      |
|      |      | the user to  |                  |   |   |    |      |
|      |      | provide key  |                  |   |   |    |      |
|      |      | deposit (in  |                  |   |   |    |      |
|      |      | lovelace)    |                  |   |   |    |      |
|      |      | that was     |                  |   |   |    |      |
|      |      | paid by the  |                  |   |   |    |      |
|      |      | target stake |                  |   |   |    |      |
|      |      | credential   |                  |   |   |    |      |
|      |      | when it      |                  |   |   |    |      |
|      |      | regist       |                  |   |   |    |      |
|      |      | ered]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | registration |                  |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | will be      |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | handles      |                  |   |   |    |      |
|      |      | errors       |                  |   |   |    |      |
|      |      | gracefully   |                  |   |   |    |      |
|      |      | and provides |                  |   |   |    |      |
|      |      | helpful      |                  |   |   |    |      |
|      |      | error        |                  |   |   |    |      |
|      |      | messages     |                  |   |   |    |      |
|      |      | when         |                  |   |   |    |      |
|      |      | required     |                  |   |   |    |      |
|      |      | options are  |                  |   |   |    |      |
|      |      | missing or   |                  |   |   |    |      |
|      |      | invalid      |                  |   |   |    |      |
|      |      | inputs are   |                  |   |   |    |      |
|      |      | provi        |                  |   |   |    |      |
|      |      | ded.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Detail Pending   |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | should be    |                  |   |   |    |      |
|      |      | saved on a   |                  |   |   |    |      |
|      |      | text         |                  |   |   |    |      |
|      |      | envelope     |                  |   |   |    |      |
|      |      | for          |                  |   |   |    |      |
|      |      | mat:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [{]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\"type\":   |                  |   |   |    |      |
|      |      | \"Cert       |                  |   |   |    |      |
|      |      | ificateConwa |                  |   |   |    |      |
|      |      | y\",]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\"de        |                  |   |   |    |      |
|      |      | scription\": |                  |   |   |    |      |
|      |      | \"Stake      |                  |   |   |    |      |
|      |      | Address      |                  |   |   |    |      |
|      |      | De           |                  |   |   |    |      |
|      |      | registration |                  |   |   |    |      |
|      |      | Certificat   |                  |   |   |    |      |
|      |      | e\",]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [            |                  |   |   |    |      |
|      |      | \"cborHex\": |                  |   |   |    |      |
|      |      | \"\"]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [}]{.mark}   |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | []{.mark}   |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Detail Pending   |   |   |    |      |
|      |      | resulting    |                  |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | conforms     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl, |                  |   |   |    |      |
|      |      | where\       |                  |   |   |    |      |
|      |      | \            |                  |   |   |    |      |
|      |      | unreg_cert = |                  |   |   |    |      |
|      |      | (8,          |                  |   |   |    |      |
|      |      | stake        |                  |   |   |    |      |
|      |      | _credential, |                  |   |   |    |      |
|      |      | c            |                  |   |   |    |      |
|      |      | oin)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [Allows the  | Detail Pending   |   |   |    |      |
| LI29 | an   | user to      |                  |   |   |    |      |
|      | ada  | provide      |                  |   |   |    |      |
|      | ho   | credentials  |                  |   |   |    |      |
|      | lder | in any of    |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      | I    | following    |                  |   |   |    |      |
|      | want | fo           |                  |   |   |    |      |
|      | to   | rms:]{.mark} |                  |   |   |    |      |
|      | dele |              |                  |   |   |    |      |
|      | gate | > [Stake     |                  |   |   |    |      |
|      | my   | >            |                  |   |   |    |      |
|      | v    | verification |                  |   |   |    |      |
|      | otes | >            |                  |   |   |    |      |
|      | to a |  key]{.mark} |                  |   |   |    |      |
|      | DRep | >            |                  |   |   |    |      |
|      | (re  | > [Stake     |                  |   |   |    |      |
|      | gist | >            |                  |   |   |    |      |
|      | ered | verification |                  |   |   |    |      |
|      | or   | > key        |                  |   |   |    |      |
|      | defa | >            |                  |   |   |    |      |
|      | ult) | file]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      | So   | > [Stake     |                  |   |   |    |      |
|      | that | > add        |                  |   |   |    |      |
|      | my   | ress]{.mark} |                  |   |   |    |      |
|      | s    | >            |                  |   |   |    |      |
|      | take | > [Stake     |                  |   |   |    |      |
|      | is   | > script     |                  |   |   |    |      |
|      | cou  | >            |                  |   |   |    |      |
|      | nted | file]{.mark} |                  |   |   |    |      |
|      | when |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | DRep |              |                  |   |   |    |      |
|      | v    |              |                  |   |   |    |      |
|      | ote. |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | S    |              |                  |   |   |    |      |
|      | take |              |                  |   |   |    |      |
|      | -add |              |                  |   |   |    |      |
|      | ress |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [When        | Detail Pending   |   |   |    |      |
|      |      | delegating   |                  |   |   |    |      |
|      |      | to a         |                  |   |   |    |      |
|      |      | registered   |                  |   |   |    |      |
|      |      | DRep, the    |                  |   |   |    |      |
|      |      | user can     |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | target Drep  |                  |   |   |    |      |
|      |      | with:\       |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [DRep      |                  |   |   |    |      |
|      |      | > script     |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [DRep      |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  key]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [DRep      |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | > key        |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [DRep key  |                  |   |   |    |      |
|      |      | > hash (Drep |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  ID)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [When        | Detail Pending   |   |   |    |      |
|      |      | delegating   |                  |   |   |    |      |
|      |      | to a default |                  |   |   |    |      |
|      |      | DRep the     |                  |   |   |    |      |
|      |      | user can use |                  |   |   |    |      |
|      |      | a flag to    |                  |   |   |    |      |
|      |      | select       |                  |   |   |    |      |
|      |      | either       |                  |   |   |    |      |
|      |      | al           |                  |   |   |    |      |
|      |      | ways-abstain |                  |   |   |    |      |
|      |      | or           |                  |   |   |    |      |
|      |      | always-no    |                  |   |   |    |      |
|      |      | -confidence, |                  |   |   |    |      |
|      |      | but not      |                  |   |   |    |      |
|      |      | b            |                  |   |   |    |      |
|      |      | oth.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | vote         |                  |   |   |    |      |
|      |      | delegation   |                  |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | will be      |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | handles      |                  |   |   |    |      |
|      |      | errors       |                  |   |   |    |      |
|      |      | gracefully   |                  |   |   |    |      |
|      |      | and provides |                  |   |   |    |      |
|      |      | helpful      |                  |   |   |    |      |
|      |      | error        |                  |   |   |    |      |
|      |      | messages     |                  |   |   |    |      |
|      |      | when         |                  |   |   |    |      |
|      |      | required     |                  |   |   |    |      |
|      |      | options are  |                  |   |   |    |      |
|      |      | missing or   |                  |   |   |    |      |
|      |      | invalid      |                  |   |   |    |      |
|      |      | inputs are   |                  |   |   |    |      |
|      |      | provi        |                  |   |   |    |      |
|      |      | ded.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Detail Pending   |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | should be    |                  |   |   |    |      |
|      |      | saved on a   |                  |   |   |    |      |
|      |      | text         |                  |   |   |    |      |
|      |      | envelope     |                  |   |   |    |      |
|      |      | for          |                  |   |   |    |      |
|      |      | mat:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [{]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\"type\":   |                  |   |   |    |      |
|      |      | \"Cert       |                  |   |   |    |      |
|      |      | ificateConwa |                  |   |   |    |      |
|      |      | y\",]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\"de        |                  |   |   |    |      |
|      |      | scription\": |                  |   |   |    |      |
|      |      | \"Vote       |                  |   |   |    |      |
|      |      | Delegation   |                  |   |   |    |      |
|      |      | Certificat   |                  |   |   |    |      |
|      |      | e\",]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [            |                  |   |   |    |      |
|      |      | \"cborHex\": |                  |   |   |    |      |
|      |      | \"\"]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [}]{.mark}   |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | []{.mark}   |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Detail Pending   |   |   |    |      |
|      |      | resulting    |                  |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | conforms     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl, |                  |   |   |    |      |
|      |      | where\       |                  |   |   |    |      |
|      |      | \            |                  |   |   |    |      |
|      |      | vot          |                  |   |   |    |      |
|      |      | e_deleg_cert |                  |   |   |    |      |
|      |      | = (9,        |                  |   |   |    |      |
|      |      | stake        |                  |   |   |    |      |
|      |      | _credential, |                  |   |   |    |      |
|      |      | d            |                  |   |   |    |      |
|      |      | rep)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [Allows the  | Detail Pending   |   |   |    |      |
| LI30 | an   | user to      |                  |   |   |    |      |
|      | ada  | provide      |                  |   |   |    |      |
|      | ho   | credentials  |                  |   |   |    |      |
|      | lder | in any of    |                  |   |   |    |      |
|      |      | the          |                  |   |   |    |      |
|      | I    | following    |                  |   |   |    |      |
|      | want | fo           |                  |   |   |    |      |
|      | to   | rms:]{.mark} |                  |   |   |    |      |
|      | dele |              |                  |   |   |    |      |
|      | gate | > [Stake     |                  |   |   |    |      |
|      | my   | >            |                  |   |   |    |      |
|      | s    | verification |                  |   |   |    |      |
|      | take | >            |                  |   |   |    |      |
|      | to a |  key]{.mark} |                  |   |   |    |      |
|      | s    | >            |                  |   |   |    |      |
|      | take | > [Stake     |                  |   |   |    |      |
|      | pool | >            |                  |   |   |    |      |
|      | AND  | verification |                  |   |   |    |      |
|      | my   | > key        |                  |   |   |    |      |
|      | v    | >            |                  |   |   |    |      |
|      | otes | file]{.mark} |                  |   |   |    |      |
|      | to a | >            |                  |   |   |    |      |
|      | DRep | > [Stake     |                  |   |   |    |      |
|      | (re  | > add        |                  |   |   |    |      |
|      | gist | ress]{.mark} |                  |   |   |    |      |
|      | ered | >            |                  |   |   |    |      |
|      | or   | > [Stake     |                  |   |   |    |      |
|      | defa | > script     |                  |   |   |    |      |
|      | ult) | >            |                  |   |   |    |      |
|      | with | file]{.mark} |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | si   |              |                  |   |   |    |      |
|      | ngle |              |                  |   |   |    |      |
|      | cert |              |                  |   |   |    |      |
|      | ific |              |                  |   |   |    |      |
|      | ate. |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | s    |              |                  |   |   |    |      |
|      | take |              |                  |   |   |    |      |
|      | -add |              |                  |   |   |    |      |
|      | ress |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The user    | Detail Pending   |   |   |    |      |
|      |      | can provide  |                  |   |   |    |      |
|      |      | the target   |                  |   |   |    |      |
|      |      | stake pool   |                  |   |   |    |      |
|      |      | with:\       |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [Stake     |                  |   |   |    |      |
|      |      | > pool cold  |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  key]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [Stake     |                  |   |   |    |      |
|      |      | > pool cold  |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | > key        |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [Stake     |                  |   |   |    |      |
|      |      | > pool       |                  |   |   |    |      |
|      |      | > ID]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Allows the  | Detail Pending   |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | target DRep  |                  |   |   |    |      |
|      |      | credential   |                  |   |   |    |      |
|      |      | with]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [DRep      |                  |   |   |    |      |
|      |      | > script     |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [DRep      |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  key]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [DRep      |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | > key        |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [DRep key  |                  |   |   |    |      |
|      |      | > hash (Drep |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  ID)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [When        | Detail Pending   |   |   |    |      |
|      |      | delegating   |                  |   |   |    |      |
|      |      | to a default |                  |   |   |    |      |
|      |      | DRep the     |                  |   |   |    |      |
|      |      | user can use |                  |   |   |    |      |
|      |      | a flag to    |                  |   |   |    |      |
|      |      | select       |                  |   |   |    |      |
|      |      | either       |                  |   |   |    |      |
|      |      | al           |                  |   |   |    |      |
|      |      | ways-abstain |                  |   |   |    |      |
|      |      | or           |                  |   |   |    |      |
|      |      | always-no    |                  |   |   |    |      |
|      |      | -confidence, |                  |   |   |    |      |
|      |      | but not      |                  |   |   |    |      |
|      |      | b            |                  |   |   |    |      |
|      |      | oth.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | stake and    |                  |   |   |    |      |
|      |      | vote         |                  |   |   |    |      |
|      |      | delegation   |                  |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | will be      |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | handles      |                  |   |   |    |      |
|      |      | errors       |                  |   |   |    |      |
|      |      | gracefully   |                  |   |   |    |      |
|      |      | and provides |                  |   |   |    |      |
|      |      | helpful      |                  |   |   |    |      |
|      |      | error        |                  |   |   |    |      |
|      |      | messages     |                  |   |   |    |      |
|      |      | when         |                  |   |   |    |      |
|      |      | required     |                  |   |   |    |      |
|      |      | options are  |                  |   |   |    |      |
|      |      | missing or   |                  |   |   |    |      |
|      |      | invalid      |                  |   |   |    |      |
|      |      | inputs are   |                  |   |   |    |      |
|      |      | provi        |                  |   |   |    |      |
|      |      | ded.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Detail Pending   |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | should be    |                  |   |   |    |      |
|      |      | saved on a   |                  |   |   |    |      |
|      |      | text         |                  |   |   |    |      |
|      |      | envelope     |                  |   |   |    |      |
|      |      | for          |                  |   |   |    |      |
|      |      | mat:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [{]{.mark}  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\"type\":   |                  |   |   |    |      |
|      |      | \"Cert       |                  |   |   |    |      |
|      |      | ificateConwa |                  |   |   |    |      |
|      |      | y\",]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [\"de        |                  |   |   |    |      |
|      |      | scription\": |                  |   |   |    |      |
|      |      | \"Stake and  |                  |   |   |    |      |
|      |      | Vote         |                  |   |   |    |      |
|      |      | Delegation   |                  |   |   |    |      |
|      |      | Certificat   |                  |   |   |    |      |
|      |      | e\",]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [            |                  |   |   |    |      |
|      |      | \"cborHex\": |                  |   |   |    |      |
|      |      | \"\"]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | [}]{.mark}   |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | []{.mark}   |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | Detail Pending   |   |   |    |      |
|      |      | resulting    |                  |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | conforms     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl, |                  |   |   |    |      |
|      |      | where\       |                  |   |   |    |      |
|      |      | \            |                  |   |   |    |      |
|      |      | stake_vot    |                  |   |   |    |      |
|      |      | e_deleg_cert |                  |   |   |    |      |
|      |      | = (10,       |                  |   |   |    |      |
|      |      | stake        |                  |   |   |    |      |
|      |      | _credential, |                  |   |   |    |      |
|      |      | p            |                  |   |   |    |      |
|      |      | ool_keyhash, |                  |   |   |    |      |
|      |      | d            |                  |   |   |    |      |
|      |      | rep)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [The new     | Detail Pending   |   |   |    |      |
| LI31 | any  | command is   |                  |   |   |    |      |
|      | per  | implemented  |                  |   |   |    |      |
|      | sona | as           |                  |   |   |    |      |
|      |      | cardano-cli  |                  |   |   |    |      |
|      | I    | conway query |                  |   |   |    |      |
|      | want | gov-s        |                  |   |   |    |      |
|      | to   | tate]{.mark} |                  |   |   |    |      |
|      | q    |              |                  |   |   |    |      |
|      | uery |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | n    |              |                  |   |   |    |      |
|      | odes |              |                  |   |   |    |      |
|      | for  |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | cur  |              |                  |   |   |    |      |
|      | rent |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | Go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | s    |              |                  |   |   |    |      |
|      | tate |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | in   |              |                  |   |   |    |      |
|      | form |              |                  |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | d    |              |                  |   |   |    |      |
|      | ecis |              |                  |   |   |    |      |
|      | ions |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | specify the  |                  |   |   |    |      |
|      |      | network id   |                  |   |   |    |      |
|      |      | (mainnet or  |                  |   |   |    |      |
|      |      | testnet      |                  |   |   |    |      |
|      |      | ma           |                  |   |   |    |      |
|      |      | gic)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | output will  |                  |   |   |    |      |
|      |      | be           |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The output  | Detail Pending   |   |   |    |      |
|      |      | is a JSON    |                  |   |   |    |      |
|      |      | showing, at  |                  |   |   |    |      |
|      |      | least, the   |                  |   |   |    |      |
|      |      | following    |                  |   |   |    |      |
|      |      | informat     |                  |   |   |    |      |
|      |      | ion:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [Previous  |                  |   |   |    |      |
|      |      | > protocol   |                  |   |   |    |      |
|      |      | > parame     |                  |   |   |    |      |
|      |      | ters]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [Current   |                  |   |   |    |      |
|      |      | > protocol   |                  |   |   |    |      |
|      |      | > parame     |                  |   |   |    |      |
|      |      | ters]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [Last      |                  |   |   |    |      |
|      |      | > enacted    |                  |   |   |    |      |
|      |      | > governance |                  |   |   |    |      |
|      |      | > actions    |                  |   |   |    |      |
|      |      | > IDs for    |                  |   |   |    |      |
|      |      | > committee, |                  |   |   |    |      |
|      |      | > c          |                  |   |   |    |      |
|      |      | onstitution, |                  |   |   |    |      |
|      |      | > hardfork   |                  |   |   |    |      |
|      |      | > initiation |                  |   |   |    |      |
|      |      | > and        |                  |   |   |    |      |
|      |      | > parameter  |                  |   |   |    |      |
|      |      | > upd        |                  |   |   |    |      |
|      |      | ates]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [Ratified  |                  |   |   |    |      |
|      |      | > governance |                  |   |   |    |      |
|      |      | > actions    |                  |   |   |    |      |
|      |      | > that will  |                  |   |   |    |      |
|      |      | > be enacted |                  |   |   |    |      |
|      |      | > at next    |                  |   |   |    |      |
|      |      | > epoch      |                  |   |   |    |      |
|      |      | > transi     |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [Active    |                  |   |   |    |      |
|      |      | > governance |                  |   |   |    |      |
|      |      | > actions    |                  |   |   |    |      |
|      |      | > proposals  |                  |   |   |    |      |
|      |      | > including  |                  |   |   |    |      |
|      |      | > their      |                  |   |   |    |      |
|      |      | > type,      |                  |   |   |    |      |
|      |      | > stake      |                  |   |   |    |      |
|      |      | > address    |                  |   |   |    |      |
|      |      | > that       |                  |   |   |    |      |
|      |      | > collects   |                  |   |   |    |      |
|      |      | > the        |                  |   |   |    |      |
|      |      | > deposit,   |                  |   |   |    |      |
|      |      | > governance |                  |   |   |    |      |
|      |      | > action id, |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  expiration, |                  |   |   |    |      |
|      |      | > spo, drep  |                  |   |   |    |      |
|      |      | > and cc     |                  |   |   |    |      |
|      |      | > v          |                  |   |   |    |      |
|      |      | otes]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | handles      |                  |   |   |    |      |
|      |      | errors       |                  |   |   |    |      |
|      |      | gracefully   |                  |   |   |    |      |
|      |      | and provides |                  |   |   |    |      |
|      |      | helpful      |                  |   |   |    |      |
|      |      | error        |                  |   |   |    |      |
|      |      | messages     |                  |   |   |    |      |
|      |      | when         |                  |   |   |    |      |
|      |      | required     |                  |   |   |    |      |
|      |      | options are  |                  |   |   |    |      |
|      |      | missing or   |                  |   |   |    |      |
|      |      | invalid      |                  |   |   |    |      |
|      |      | inputs are   |                  |   |   |    |      |
|      |      | provi        |                  |   |   |    |      |
|      |      | ded.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As a | [The command | Detail Pending   |   |   |    |      |
| LI32 | CC   | is           |                  |   |   |    |      |
|      | me   | implemented  |                  |   |   |    |      |
|      | mber | as           |                  |   |   |    |      |
|      |      | cardano-cli  |                  |   |   |    |      |
|      | I    | conway query |                  |   |   |    |      |
|      | want | committee-s  |                  |   |   |    |      |
|      | to   | tate]{.mark} |                  |   |   |    |      |
|      | q    |              |                  |   |   |    |      |
|      | uery |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | ommi |              |                  |   |   |    |      |
|      | ttee |              |                  |   |   |    |      |
|      | s    |              |                  |   |   |    |      |
|      | tate |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | find |              |                  |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | ex   |              |                  |   |   |    |      |
|      | pira |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | term |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | whe  |              |                  |   |   |    |      |
|      | ther |              |                  |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | hot  |              |                  |   |   |    |      |
|      | key  |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | utho |              |                  |   |   |    |      |
|      | riza |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | cer  |              |                  |   |   |    |      |
|      | tifi |              |                  |   |   |    |      |
|      | cate |              |                  |   |   |    |      |
|      | has  |              |                  |   |   |    |      |
|      | been |              |                  |   |   |    |      |
|      | reco |              |                  |   |   |    |      |
|      | rded |              |                  |   |   |    |      |
|      | on   |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Requires    | Detail Pending   |   |   |    |      |
|      |      | the user to  |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | network      |                  |   |   |    |      |
|      |      | id]{.mark}   |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Supports a  | Detail Pending   |   |   |    |      |
|      |      | query for an |                  |   |   |    |      |
|      |      | specific CC  |                  |   |   |    |      |
|      |      | credential\  |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [CC cold   |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  key]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [CC cold   |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | > key        |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [CC cold   |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | > key        |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [CC hot    |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  key]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [CC hot    |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | > key        |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [CC hot    |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | > key        |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [When no CC  | Detail Pending   |   |   |    |      |
|      |      | key is       |                  |   |   |    |      |
|      |      | specified,   |                  |   |   |    |      |
|      |      | the command  |                  |   |   |    |      |
|      |      | outputs      |                  |   |   |    |      |
|      |      | information  |                  |   |   |    |      |
|      |      | for all      |                  |   |   |    |      |
|      |      | committee    |                  |   |   |    |      |
|      |      | mem          |                  |   |   |    |      |
|      |      | bers]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | allows       |                  |   |   |    |      |
|      |      | filtering by |                  |   |   |    |      |
|      |      | active,      |                  |   |   |    |      |
|      |      | expired and  |                  |   |   |    |      |
|      |      | unrecognized |                  |   |   |    |      |
|      |      | members      |                  |   |   |    |      |
|      |      | (registered  |                  |   |   |    |      |
|      |      | hot keys to  |                  |   |   |    |      |
|      |      | an unknown   |                  |   |   |    |      |
|      |      | cc cold      |                  |   |   |    |      |
|      |      | key)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The output  | Detail Pending   |   |   |    |      |
|      |      | is a JSON    |                  |   |   |    |      |
|      |      | showing, the |                  |   |   |    |      |
|      |      | following    |                  |   |   |    |      |
|      |      | informat     |                  |   |   |    |      |
|      |      | ion:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [Cold key  |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [Hot       |                  |   |   |    |      |
|      |      | > credential |                  |   |   |    |      |
|      |      | > status     |                  |   |   |    |      |
|      |      | > (Authorize |                  |   |   |    |      |
|      |      | d/NotAuthori |                  |   |   |    |      |
|      |      | zed)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [When      |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  Authorized, |                  |   |   |    |      |
|      |      | > shows the  |                  |   |   |    |      |
|      |      | > hot key    |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [Status    |                  |   |   |    |      |
|      |      | > (Active,   |                  |   |   |    |      |
|      |      | > Expired,   |                  |   |   |    |      |
|      |      | > Unrecogni  |                  |   |   |    |      |
|      |      | zed)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  [Expiration |                  |   |   |    |      |
|      |      | > e          |                  |   |   |    |      |
|      |      | poch]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [Current   |                  |   |   |    |      |
|      |      | > epoch      |                  |   |   |    |      |
|      |      | > (when you  |                  |   |   |    |      |
|      |      | > ran the    |                  |   |   |    |      |
|      |      | > qu         |                  |   |   |    |      |
|      |      | ery)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [Qu        |                  |   |   |    |      |
|      |      | orum]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | output will  |                  |   |   |    |      |
|      |      | be           |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | handles      |                  |   |   |    |      |
|      |      | errors       |                  |   |   |    |      |
|      |      | gracefully   |                  |   |   |    |      |
|      |      | and provides |                  |   |   |    |      |
|      |      | helpful      |                  |   |   |    |      |
|      |      | error        |                  |   |   |    |      |
|      |      | messages     |                  |   |   |    |      |
|      |      | when         |                  |   |   |    |      |
|      |      | required     |                  |   |   |    |      |
|      |      | options are  |                  |   |   |    |      |
|      |      | missing or   |                  |   |   |    |      |
|      |      | invalid      |                  |   |   |    |      |
|      |      | inputs are   |                  |   |   |    |      |
|      |      | provi        |                  |   |   |    |      |
|      |      | ded.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [The command | Detail Pending   |   |   |    |      |
| LI33 | an   | is           |                  |   |   |    |      |
|      | ada  | implemented  |                  |   |   |    |      |
|      | ho   | as           |                  |   |   |    |      |
|      | lder | cardano-cli  |                  |   |   |    |      |
|      |      | conway query |                  |   |   |    |      |
|      | I    | drep-s       |                  |   |   |    |      |
|      | want | tate]{.mark} |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | q    |              |                  |   |   |    |      |
|      | uery |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | DRep |              |                  |   |   |    |      |
|      | s    |              |                  |   |   |    |      |
|      | tate |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | ...  |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Requires    | Detail Pending   |   |   |    |      |
|      |      | the user to  |                  |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | network      |                  |   |   |    |      |
|      |      | id]{.mark}   |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Supports a  | Detail Pending   |   |   |    |      |
|      |      | query for an |                  |   |   |    |      |
|      |      | specific     |                  |   |   |    |      |
|      |      | DRep         |                  |   |   |    |      |
|      |      | creden       |                  |   |   |    |      |
|      |      | tial]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [DRep      |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  key]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [DRep      |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | > key        |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [DRep      |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | > key hash   |                  |   |   |    |      |
|      |      | > (DRep      |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  ID)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [If no Drep  | Detail Pending   |   |   |    |      |
|      |      | credential   |                  |   |   |    |      |
|      |      | is specified |                  |   |   |    |      |
|      |      | it returns   |                  |   |   |    |      |
|      |      | all          |                  |   |   |    |      |
|      |      | D            |                  |   |   |    |      |
|      |      | Reps]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | output will  |                  |   |   |    |      |
|      |      | be           |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The output  | Detail Pending   |   |   |    |      |
|      |      | is a JSON    |                  |   |   |    |      |
|      |      | showing, the |                  |   |   |    |      |
|      |      | following    |                  |   |   |    |      |
|      |      | i            |                  |   |   |    |      |
|      |      | nformation:\ |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [Drep Key  |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [Anchor    |                  |   |   |    |      |
|      |      | > (Drep      |                  |   |   |    |      |
|      |      | > metad      |                  |   |   |    |      |
|      |      | ata)]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [Dep       |                  |   |   |    |      |
|      |      | osit]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [Expiry    |                  |   |   |    |      |
|      |      | > (from Drep |                  |   |   |    |      |
|      |      | > activ      |                  |   |   |    |      |
|      |      | ity)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | handles      |                  |   |   |    |      |
|      |      | errors       |                  |   |   |    |      |
|      |      | gracefully   |                  |   |   |    |      |
|      |      | and provides |                  |   |   |    |      |
|      |      | helpful      |                  |   |   |    |      |
|      |      | error        |                  |   |   |    |      |
|      |      | messages     |                  |   |   |    |      |
|      |      | when         |                  |   |   |    |      |
|      |      | required     |                  |   |   |    |      |
|      |      | options are  |                  |   |   |    |      |
|      |      | missing or   |                  |   |   |    |      |
|      |      | invalid      |                  |   |   |    |      |
|      |      | inputs are   |                  |   |   |    |      |
|      |      | provi        |                  |   |   |    |      |
|      |      | ded.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [The command | Detail Pending   |   |   |    |      |
| LI34 | an   | is           |                  |   |   |    |      |
|      | ada  | implemented  |                  |   |   |    |      |
|      | ho   | as           |                  |   |   |    |      |
|      | lder | cardano-cli  |                  |   |   |    |      |
|      | and  | conway query |                  |   |   |    |      |
|      | DRep | drep-st      |                  |   |   |    |      |
|      |      | ake-distribu |                  |   |   |    |      |
|      | I    | tion]{.mark} |                  |   |   |    |      |
|      | want |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | q    |              |                  |   |   |    |      |
|      | uery |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | DRep |              |                  |   |   |    |      |
|      | s    |              |                  |   |   |    |      |
|      | take |              |                  |   |   |    |      |
|      | dist |              |                  |   |   |    |      |
|      | ribu |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | So   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | find |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | we   |              |                  |   |   |    |      |
|      | ight |              |                  |   |   |    |      |
|      | (of  |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | vo   |              |                  |   |   |    |      |
|      | tes) |              |                  |   |   |    |      |
|      | of   |              |                  |   |   |    |      |
|      | each |              |                  |   |   |    |      |
|      | DRep |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Supports a  | Detail Pending   |   |   |    |      |
|      |      | query for an |                  |   |   |    |      |
|      |      | specific     |                  |   |   |    |      |
|      |      | DRep         |                  |   |   |    |      |
|      |      | creden       |                  |   |   |    |      |
|      |      | tial]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [DRep      |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  key]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [DRep      |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | > key        |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | file]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [DRep      |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | verification |                  |   |   |    |      |
|      |      | > key hash   |                  |   |   |    |      |
|      |      | > (DRep      |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  ID)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [If no Drep  | Detail Pending   |   |   |    |      |
|      |      | credential   |                  |   |   |    |      |
|      |      | is specified |                  |   |   |    |      |
|      |      | it returns   |                  |   |   |    |      |
|      |      | all          |                  |   |   |    |      |
|      |      | D            |                  |   |   |    |      |
|      |      | Reps]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | has the flag |                  |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | output will  |                  |   |   |    |      |
|      |      | be           |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The output  | Detail Pending   |   |   |    |      |
|      |      | is a JSON    |                  |   |   |    |      |
|      |      | showing, the |                  |   |   |    |      |
|      |      | following    |                  |   |   |    |      |
|      |      | i            |                  |   |   |    |      |
|      |      | nformation:\ |                  |   |   |    |      |
|      |      | ]{.mark}     |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [Drep Key  |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | hash]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [Stake     |                  |   |   |    |      |
|      |      | > delegated  |                  |   |   |    |      |
|      |      | > to this    |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | DRep]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | Detail Pending   |   |   |    |      |
|      |      | handles      |                  |   |   |    |      |
|      |      | errors       |                  |   |   |    |      |
|      |      | gracefully   |                  |   |   |    |      |
|      |      | and provides |                  |   |   |    |      |
|      |      | helpful      |                  |   |   |    |      |
|      |      | error        |                  |   |   |    |      |
|      |      | messages     |                  |   |   |    |      |
|      |      | when         |                  |   |   |    |      |
|      |      | required     |                  |   |   |    |      |
|      |      | options are  |                  |   |   |    |      |
|      |      | missing or   |                  |   |   |    |      |
|      |      | invalid      |                  |   |   |    |      |
|      |      | inputs are   |                  |   |   |    |      |
|      |      | provi        |                  |   |   |    |      |
|      |      | ded.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [Expand the  |                  |   |   |    |      |
| LI35 | an   | command      |                  |   |   |    |      |
|      | ada  | query        |                  |   |   |    |      |
|      | hol  | stake-       |                  |   |   |    |      |
|      | der, | address-info |                  |   |   |    |      |
|      |      | to return    |                  |   |   |    |      |
|      | I    | the drep id  |                  |   |   |    |      |
|      | want | of the DRep  |                  |   |   |    |      |
|      | to   | that the     |                  |   |   |    |      |
|      | q    | stake        |                  |   |   |    |      |
|      | uery | credential   |                  |   |   |    |      |
|      | my   | is delegated |                  |   |   |    |      |
|      | s    | to and the   |                  |   |   |    |      |
|      | take | value of the |                  |   |   |    |      |
|      | add  | existing     |                  |   |   |    |      |
|      | ress | depos        |                  |   |   |    |      |
|      | inf  | its.]{.mark} |                  |   |   |    |      |
|      | orma |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | so   |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | l    |              |                  |   |   |    |      |
|      | earn |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | w    |              |                  |   |   |    |      |
|      | hich |              |                  |   |   |    |      |
|      | pool |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | drep |              |                  |   |   |    |      |
|      | Im   |              |                  |   |   |    |      |
|      | de   |              |                  |   |   |    |      |
|      | lega |              |                  |   |   |    |      |
|      | ting |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | v    |              |                  |   |   |    |      |
|      | alue |              |                  |   |   |    |      |
|      | in   |              |                  |   |   |    |      |
|      | love |              |                  |   |   |    |      |
|      | lace |              |                  |   |   |    |      |
|      | of   |              |                  |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | depo |              |                  |   |   |    |      |
|      | sits |              |                  |   |   |    |      |
|      | for  |              |                  |   |   |    |      |
|      | de   |              |                  |   |   |    |      |
|      | lega |              |                  |   |   |    |      |
|      | ting |              |                  |   |   |    |      |
|      | and  |              |                  |   |   |    |      |
|      | for  |              |                  |   |   |    |      |
|      | su   |              |                  |   |   |    |      |
|      | bmit |              |                  |   |   |    |      |
|      | ting |              |                  |   |   |    |      |
|      | go   |              |                  |   |   |    |      |
|      | vern |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | acti |              |                  |   |   |    |      |
|      | ons. |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      | Sc   |              |                  |   |   |    |      |
|      | ript |              |                  |   |   |    |      |
|      | as a |              |                  |   |   |    |      |
|      | DRep |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| S    |      |              |                  |   |   |    |      |
| idec |      |              |                  |   |   |    |      |
| hain |      |              |                  |   |   |    |      |
| User |      |              |                  |   |   |    |      |
| Sto  |      |              |                  |   |   |    |      |
| ries |      |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CH.  | As a | [[Jon        | Detail Pending   |   | D | S  |      |
| SID1 | Si   | Rossie       |                  |   | e | id |      |
|      | dech | ]{.underline |                  |   | t | ec |      |
|      | ain, | }](mailto:jo |                  |   | a | ha |      |
|      | I    | n.rossie@ioh |                  |   | i | in |      |
|      | wish | k.io)[posted |                  |   | l |    |      |
|      | to   | your 'thread |                  |   | P |    |      |
|      | use  | comments' to |                  |   | e |    |      |
|      | BLS  | init         |                  |   | n |    |      |
|      | pr   | iate]{.mark} |                  |   | d |    |      |
|      | imit |              |                  |   | i |    |      |
|      | ives |              |                  |   | n |    |      |
|      | to   |              |                  |   | g |    |      |
|      | re   |              |                  |   |   |    |      |
|      | cord |              |                  |   |   |    |      |
|      | se   |              |                  |   |   |    |      |
|      | ttle |              |                  |   |   |    |      |
|      | ment |              |                  |   |   |    |      |
|      | op   |              |                  |   |   |    |      |
|      | erat |              |                  |   |   |    |      |
|      | ions |              |                  |   |   |    |      |
|      | on   |              |                  |   |   |    |      |
|      | Car  |              |                  |   |   |    |      |
|      | dano |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CH.  | S    | Detail       | Detail Pending   |   | D | S  |      |
| SID2 | idec | Pending      |                  |   | e | id |      |
|      | hain |              |                  |   | t | ec |      |
|      | will |              |                  |   | a | ha |      |
|      | use  |              |                  |   | i | in |      |
|      | BLS  |              |                  |   | l |    |      |
|      | for  |              |                  |   | P |    |      |
|      | tok  |              |                  |   | e |    |      |
|      | enom |              |                  |   | n |    |      |
|      | ics, |              |                  |   | d |    |      |
|      | in   |              |                  |   | i |    |      |
|      | pa   |              |                  |   | n |    |      |
|      | rtic |              |                  |   | g |    |      |
|      | ular |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | sup  |              |                  |   |   |    |      |
|      | port |              |                  |   |   |    |      |
|      | m    |              |                  |   |   |    |      |
|      | ulti |              |                  |   |   |    |      |
|      | -sig |              |                  |   |   |    |      |
|      | cert |              |                  |   |   |    |      |
|      | ific |              |                  |   |   |    |      |
|      | ates |              |                  |   |   |    |      |
|      | a    |              |                  |   |   |    |      |
|      | bout |              |                  |   |   |    |      |
|      | S    |              |                  |   |   |    |      |
|      | idec |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
|      | acti |              |                  |   |   |    |      |
|      | vity |              |                  |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | veri |              |                  |   |   |    |      |
|      | fied |              |                  |   |   |    |      |
|      | by   |              |                  |   |   |    |      |
|      | Pl   |              |                  |   |   |    |      |
|      | utus |              |                  |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
|      | ontr |              |                  |   |   |    |      |
|      | acts |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| Pl   |      |              |                  |   |   |    |      |
| utus |      |              |                  |   |   |    |      |
| C    |      |              |                  |   |   |    |      |
| ompo |      |              |                  |   |   |    |      |
| nent |      |              |                  |   |   |    |      |
| L    |      |              |                  |   |   |    |      |
| evel |      |              |                  |   |   |    |      |
| User |      |              |                  |   |   |    |      |
| Sto  |      |              |                  |   |   |    |      |
| ries |      |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CI   | As a | Sums         | Detail Pending   |   |   | Pl |      |
| P-85 | DApp | -of-products |                  |   |   | ut |      |
|      | d    | is available |                  |   |   | us |      |
|      | evel | to use in    |                  |   |   |    |      |
|      | oper | Plutus V3    |                  |   |   |    |      |
|      | I    | scripts and  |                  |   |   |    |      |
|      | w    | is the       |                  |   |   |    |      |
|      | ould | default way  |                  |   |   |    |      |
|      | like | of encoding  |                  |   |   |    |      |
|      | to   | data types   |                  |   |   |    |      |
|      | use  | in Plutus    |                  |   |   |    |      |
|      | sums | Tx.          |                  |   |   |    |      |
|      | -of- |              |                  |   |   |    |      |
|      | prod |              |                  |   |   |    |      |
|      | ucts |              |                  |   |   |    |      |
|      | ins  |              |                  |   |   |    |      |
|      | tead |              |                  |   |   |    |      |
|      | of   |              |                  |   |   |    |      |
|      | Sc   |              |                  |   |   |    |      |
|      | ott- |              |                  |   |   |    |      |
|      | enco |              |                  |   |   |    |      |
|      | ding |              |                  |   |   |    |      |
|      | in   |              |                  |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | Pl   |              |                  |   |   |    |      |
|      | utus |              |                  |   |   |    |      |
|      | scr  |              |                  |   |   |    |      |
|      | ipts |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | get  |              |                  |   |   |    |      |
|      | be   |              |                  |   |   |    |      |
|      | tter |              |                  |   |   |    |      |
|      | per  |              |                  |   |   |    |      |
|      | form |              |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CIP  | User | Detail       | Detail Pending   |   |   | Pl |      |
| -101 | sto  | Pending      |                  |   |   | ut |      |
|      | ries |              |                  |   |   | us |      |
|      | for  |              |                  |   |   |    |      |
|      | K    |              |                  |   |   |    |      |
|      | ecca |              |                  |   |   |    |      |
|      | k256 |              |                  |   |   |    |      |
|      | p    |              |                  |   |   |    |      |
|      | rimi |              |                  |   |   |    |      |
|      | tive |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      | As a | The          | Detail Pending   |   |   | Pl |      |
|      | DApp | Blake2b-224  |                  |   |   | ut |      |
|      | d    | is available |                  |   |   | us |      |
|      | evel | to use in    |                  |   |   |    |      |
|      | oper | Plutus V3    |                  |   |   |    |      |
|      | I    | after the HF |                  |   |   |    |      |
|      | want |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | use  |              |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | Bla  |              |                  |   |   |    |      |
|      | ke2b |              |                  |   |   |    |      |
|      | -224 |              |                  |   |   |    |      |
|      | has  |              |                  |   |   |    |      |
|      | hing |              |                  |   |   |    |      |
|      | func |              |                  |   |   |    |      |
|      | tion |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | com  |              |                  |   |   |    |      |
|      | pute |              |                  |   |   |    |      |
|      | Pu   |              |                  |   |   |    |      |
|      | bKey |              |                  |   |   |    |      |
|      | Hash |              |                  |   |   |    |      |
|      | onc  |              |                  |   |   |    |      |
|      | hain |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+

# Revision & Approval

  -----------------------------------------------------------------------------------------------------------------------
  Name                                                        Position       Role       Comments           Status
  ----------------------------------------------------------- -------------- ---------- ------------------ --------------
  [[Mike Ward]{.underline}](mailto:mike.ward@iohk.io)         Chief Product  Approver                      Under Review
                                                              Officer                                      

  [[Michael                                                   Product        Approver                      Under Review
  Madoff]{.underline}](mailto:michael.madoff@iohk.io)         Manager -                                    
                                                              Voltaire                                     

  [[Samuel                                                    Product        Approver                      Under Review
  Leathers]{.underline}](mailto:samuel.leathers@iohk.io)      Manager - Core                               
                                                              Tech                                         

  [[Dorin Solomon]{.underline}](mailto:dorin.solomon@iohk.io) Quality        Approver                      
                                                              Chapter                                      
                                                              Director                                     

  [[Carlos Lopez de                                           Product        Reviewer                      Under Review
  Lara]{.underline}](mailto:carlos.lopezdelara@iohk.io)       Owner - Core                                 
                                                              Tech                                         

  [[Kevin Hammond]{.underline}](mailto:kevin.hammond@iohk.io) Head of        Approver                      Under Review
                                                              Technology -                                 
                                                              Core Tech                                    

  [[Lorenzo Bruno]{.underline}](mailto:lorenzo.bruno@iohk.io) Product Design Reviewer                      
                                                              Lead -                                       
                                                              Voltaire                                     
                                                              Governance                                   
                                                              Tools                                        

  [[Thomas                                                    Product        Reviewer                      Under Review
  Upfield]{.underline}](mailto:thomas.upfield@iohk.io)        Owner -                                      
                                                              Voltaire                                     

  [[Gerard                                                    COO            Reviewer                      Under Review
  Moroney]{.underline}](mailto:gerard.moroney@iohk.io)                                                     

  [[Omer Husain]{.underline}](mailto:omer.husain@iohk.io)     Product        Reviewer   Confirm Smart      To Be Added
                                                              Manager -                 Contracts User     
                                                              Plutus                    Stories            

  [[Billy Mullins]{.underline}](mailto:billy.mullins@iohk.io) VP Cardano     Reviewer   Confirm All User   Under Review
                                                                                        Stories            

  [[Dominik                                                   Sidechains     Reviewer   Confirm Sidechains Detail Pending
  Zajkowski]{.underline}](mailto:dominik.zajkowski@iohk.io)   Architect                 User Stories       

  [[Arnaud Bailly]{.underline}](mailto:arnaud.bailly@iohk.io) Hydra          Reviewer   Confirm Hydra User 
                                                              Architect                 Stories            
  -----------------------------------------------------------------------------------------------------------------------

# 
