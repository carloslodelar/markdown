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

  ------------------------------------------------------
  **Source**   **Outline        **State**   **Key
               Contribution**               Contract**
  ------------ ---------------- ----------- ------------
  Voltaire     Use Cases for    Initial     Outreach in
               Governance,      Capture     progress
               voting,          Complete
               delegation

  CIP-1694     Blockchain level Initial     Outreach in
               User Stories on  Capture     progress
               voting,          Complete
               delegation,
               identity,
               consensus

  Smart        Plutus v3 and    Initial     Outreach in
  Contracts    BLS              Capture     progress
                                Complete

  CLI-API      Interface        Initial     Outreach in
               outline and      Capture     progress
               definition       Complete

  Sidechains   Interaction with Outreach in Outreach in
               BLS primitives   progress    progress

  DApps        To be defined    To be       Outreach in
               and elaborated   defined     progress

  Exchanges    To be defined    To be       Outreach in
               and elaborated   defined     progress

  Other        To be defined    To be       Outreach in
               and elaborated   defined     progress
  ------------------------------------------------------

# User Story (Voltaire, API, CIP-1694, Community et al)

+------+------+--------------+------------------+---+---+----+------+
| **U  | **   | **Functional | **Acceptance     | * | * | ** | **En |
| ID** | User | R            | Criteria**       | * | * | So | able |
|      | Sto  | equirement** |                  | L | A | ur | r(Y, |
|      | ry** |              |                  | i | c | ce | N)** |
|      |      |              |                  | n | c | ** |      |
|      |      |              |                  | k | e |    |      |
|      |      |              |                  | * | p |    |      |
|      |      |              |                  | * | t |    |      |
|      |      |              |                  |   | e |    |      |
|      |      |              |                  |   | d |    |      |
|      |      |              |                  |   | * |    |      |
|      |      |              |                  |   | * |    |      |
+======+======+==============+==================+===+===+====+======+
| CH   | As a | Connect with | Given I am on    |   |   | Vo | N    |
| .VO1 | DRep | multiple     | the homepage     |   |   | lt |      |
|      | or   | stake key    |                  |   |   | ai |      |
|      | Ada  | wallet       | And my wallet is |   |   | re |      |
|      | Ho   |              | not connected.   |   |   |    |      |
|      | lder |              |                  |   |   |    |      |
|      | **I  |              | When I click the |   |   |    |      |
|      | want |              | Connect Wallet   |   |   |    |      |
|      | to   |              | button           |   |   |    |      |
|      | con  |              |                  |   |   |    |      |
|      | nect |              | And select (one  |   |   |    |      |
|      | my   |              | of) my CIP-95    |   |   |    |      |
|      | wa   |              | compatible       |   |   |    |      |
|      | llet |              | wallet(s) with   |   |   |    |      |
|      | to   |              | multiple stake   |   |   |    |      |
|      | G    |              | keys             |   |   |    |      |
|      | ovTo |              |                  |   |   |    |      |
|      | ol** |              | And select from  |   |   |    |      |
|      | so   |              | a list which     |   |   |    |      |
|      | that |              | stake key I wish |   |   |    |      |
|      | I    |              | to connect with  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | post |              | Then the wallet  |   |   |    |      |
|      | tran |              | will prompt me   |   |   |    |      |
|      | sact |              | to connect and I |   |   |    |      |
|      | ions |              | can connect to   |   |   |    |      |
|      | on-c |              | GovTool with it  |   |   |    |      |
|      | hain |              | on the selected  |   |   |    |      |
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
|      | **I  |              | page             |   |   |    |      |
|      | want |              |                  |   |   |    |      |
|      | to** |              | When I select    |   |   |    |      |
|      | **   |              | the delegate to  |   |   |    |      |
|      | dele |              | DRep ID option   |   |   |    |      |
|      | gate |              | and I enter a    |   |   |    |      |
|      | my   |              | DRep ID which    |   |   |    |      |
|      | vo   |              | has not been     |   |   |    |      |
|      | ting |              | registered and I |   |   |    |      |
|      | pow  |              | press delegate   |   |   |    |      |
|      | er** |              |                  |   |   |    |      |
|      | to a |              | Then I will be   |   |   |    |      |
|      | DRep |              | presented with   |   |   |    |      |
|      | so   |              | an error message |   |   |    |      |
|      | that |              | explaining that  |   |   |    |      |
|      | I    |              | the DRep ID was  |   |   |    |      |
|      | can  |              | not found.       |   |   |    |      |
|      | c    |              |                  |   |   |    |      |
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
|      |      | disconnected | DRep wallet      |   |   | ai |      |
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
|      |      |              | delegated and it |   |   |    |      |
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
|      |      |              | transaction was  |   |   |    |      |
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
|      |      |              | transaction was  |   |   |    |      |
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
|      |      |              | transaction was  |   |   |    |      |
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
|      |      |              | transaction was  |   |   |    |      |
|      |      |              | sent.            |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | Guardrails   | This work is in  |   |   | Vo |      |
|      |      | for Voltaire | progress         |   |   | lt |      |
|      |      |              |                  |   |   | ai |      |
|      |      |              |                  |   |   | re |      |
+------+------+--------------+------------------+---+---+----+------+
| CH   | **As | Register as  | Given that I am  |   |   | Vo | N    |
| .VO3 | a    | a DRep       | connected to     |   |   | lt |      |
|      | DRep |              | GovTool with a   |   |   | ai |      |
|      | I    |              | compatible       |   |   | re |      |
|      | want |              | wallet           |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | re   |              | When I go        |   |   |    |      |
|      | gist |              | through the DRep |   |   |    |      |
|      | er** |              | registration     |   |   |    |      |
|      | so   |              | process, and do  |   |   |    |      |
|      | that |              | not include a    |   |   |    |      |
|      | I    |              | metadata anchor  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | vote |              | Then I can       |   |   |    |      |
|      | on   |              | register as a    |   |   |    |      |
|      | go   |              | DRep via my      |   |   |    |      |
|      | vern |              | wallet (because  |   |   |    |      |
|      | ance |              | metadata anchors |   |   |    |      |
|      | act  |              | are optional)    |   |   |    |      |
|      | ions |              |                  |   |   |    |      |
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
| CH   | **As | Should be    | Given that I am  |   |   | Vo | N    |
| .VO4 | a    | able to      | a DRep and I am  |   |   | lt |      |
|      | DRep | access the   | connected to     |   |   | ai |      |
|      | I    | governance   | GovTool          |   |   | re |      |
|      | want | actions page |                  |   |   |    |      |
|      | to   | as a DRep    | When I visit the |   |   |    |      |
|      | vo   | with my      | url of the       |   |   |    |      |
|      | te** | wallet       | governance       |   |   |    |      |
|      | so   | connected    | actions page     |   |   |    |      |
|      | that |              |                  |   |   |    |      |
|      | I    |              | Then the         |   |   |    |      |
|      | can  |              | governance       |   |   |    |      |
|      | fu   |              | actions page is  |   |   |    |      |
|      | lfil |              | displayed        |   |   |    |      |
|      | my   |              |                  |   |   |    |      |
|      | role |              |                  |   |   |    |      |
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
| CH   | **As | Only a user  | Given that I am  |   |   | Vo | N    |
| .VO5 | a    | who is       | not registered   |   |   | lt |      |
|      | DRep | registered   | as a DRep,       |   |   | ai |      |
|      | I    | as a DRep    |                  |   |   | re |      |
|      | want | can retire   | When I look for  |   |   |    |      |
|      | to   |              | a retirement     |   |   |    |      |
|      | reti |              | option in        |   |   |    |      |
|      | re** |              | GovTool          |   |   |    |      |
|      | so   |              |                  |   |   |    |      |
|      | that |              | Then there is    |   |   |    |      |
|      | I    |              | none.            |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
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
| CH   | **As | A DRep can   | Given that I am  |   |   | Vo | N    |
| .VO6 | a    | update their | a DRep and am    |   |   | lt |      |
|      | DRep | registration | connected to     |   |   | ai |      |
|      | I    | after        | GovTool and am   |   |   | re |      |
|      | want | registering  | on the           |   |   |    |      |
|      | to   |              | dashboard.       |   |   |    |      |
|      | up   |              |                  |   |   |    |      |
|      | date |              | Then when I      |   |   |    |      |
|      | my   |              | click the        |   |   |    |      |
|      | d    |              | "change          |   |   |    |      |
|      | etai |              | metadata" button |   |   |    |      |
|      | ls** |              | on the DRep tab. |   |   |    |      |
|      | so   |              |                  |   |   |    |      |
|      | that |              | Then I am        |   |   |    |      |
|      | I    |              | directed to      |   |   |    |      |
|      | can  |              | update my        |   |   |    |      |
|      | be   |              | metadata and can |   |   |    |      |
|      | tter |              | submit a DRep    |   |   |    |      |
|      | a    |              | update           |   |   |    |      |
|      | dver |              | certificate to   |   |   |    |      |
|      | tise |              | register this    |   |   |    |      |
|      | my   |              | on-chain.        |   |   |    |      |
|      | self |              |                  |   |   |    |      |
|      | to   |              |                  |   |   |    |      |
|      | Ada  |              |                  |   |   |    |      |
|      | Hol  |              |                  |   |   |    |      |
|      | ders |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CH   | As   | Anyone       | Given that I am  |   |   | Vo | N    |
| .VO7 | any  | should be    | on the GovTool   |   |   | lt |      |
|      | user | able to      | homepage,        |   |   | ai |      |
|      | **I  | access the   |                  |   |   | re |      |
|      | want | governance   | When I click the |   |   |    |      |
|      | to   | actions page | "Governance      |   |   |    |      |
|      | view | without a    | actions" in the  |   |   |    |      |
|      | go   | wallet       | topbar           |   |   |    |      |
|      | vern | connected    |                  |   |   |    |      |
|      | ance |              | Then I am sent   |   |   |    |      |
|      | a    |              | to the           |   |   |    |      |
|      | ctio |              | governance       |   |   |    |      |
|      | ns** |              | actions page.    |   |   |    |      |
|      | so I |              |                  |   |   |    |      |
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
|      | **I  |              |                  |   |   |    |      |
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
|      | Memb |              |                  |   |   |    |      |
|      | er** |              |                  |   |   |    |      |
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
|      |      |              | I run the        |   |   | [* |      |
|      |      |              | corresponding    |   |   | *[ |      |
|      |      |              | command, then I  |   |   | L9 |      |
|      |      |              | can verify that  |   |   | 93 |      |
|      |      |              | the certificate  |   |   | ]{ |      |
|      |      |              | is stored        |   |   | .u |      |
|      |      |              | on-chain and it  |   |   | nd |      |
|      |      |              | delegates rights |   |   | er |      |
|      |      |              | from the cold    |   |   | li |      |
|      |      |              | key to the hot   |   |   | ne |      |
|      |      |              | key              |   |   | }* |      |
|      |      |              |                  |   |   | *] |      |
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
|      |      | Only votes   | Given that my    |   |   | CI | N    |
|      |      | from active  | set of keys does |   |   | P- |      |
|      |      | Committee    | not correspond   |   |   | 16 |      |
|      |      | members are  | to an active CC  |   |   | 94 |      |
|      |      | considered.  | member, when I   |   |   |    |      |
|      |      |              | try to vote as a |   |   | [* |      |
|      |      |              | CC member using  |   |   | *[ |      |
|      |      |              | CLI, then I get  |   |   | L9 |      |
|      |      |              | an error message |   |   | 93 |      |
|      |      |              | telling me that  |   |   | ]{ |      |
|      |      |              | my credentials   |   |   | .u |      |
|      |      |              | are not valid    |   |   | nd |      |
|      |      |              |                  |   |   | er |      |
|      |      |              |                  |   |   | li |      |
|      |      |              |                  |   |   | ne |      |
|      |      |              |                  |   |   | }* |      |
|      |      |              |                  |   |   | *] |      |
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
| CH   | **As | Access       | Given that I am  |   |   | Vo | N    |
| .VO9 | a CC | GovTool      | on the GovTool   |   |   | lt |      |
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
|      | acti |              |                  |   |   |    |      |
|      | on** |              |                  |   |   |    |      |
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
| CH.  | **As | Find a       | Given that I am  |   |   | Vo | N    |
| VO10 | a CC | specific     | using CLI and I  |   |   | lt |      |
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
|      | acti |              | details of that  |   |   |    |      |
|      | on** |              | individual       |   |   |    |      |
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
| CH.  | **As | Create a new | Given that I am  |   |   | Vo | N    |
| VO11 | a CC | a            | a CC member and  |   |   | lt |      |
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
|      | c    |              | authorised to    |   |   |    |      |
|      | rede |              | vote as a valid  |   |   |    |      |
|      | ntia |              | CC member        |   |   |    |      |
|      | ls** |              |                  |   |   |    |      |
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
| CH.  | **As | Create a     | Given that I am  |   |   | Vo | N    |
| VO12 | a CC | resignation  | a CC member and  |   |   | lt |      |
|      | Me   | certificate  | I have enough    |   |   | ai |      |
|      | mber |              | funds to pay the |   |   | re |      |
|      | I    |              | transaction      |   |   |    |      |
|      | want |              | fees, When I     |   |   |    |      |
|      | to   |              | create a         |   |   |    |      |
|      | reti |              | resignation      |   |   |    |      |
|      | re** |              | certificate,     |   |   |    |      |
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
| CH.  | **As | *Correct     | Detail pending   |   | D | A  |      |
| CLI1 | a    | operation of |                  |   | e | PI |      |
|      | Pl   | BLS          |                  |   | t | /C |      |
|      | utus | primitives.* |                  |   | a | LI |      |
|      | d    |              |                  |   | i |    |      |
|      | evel | *Correct     |                  |   | l |    |      |
|      | oper | operation of |                  |   | p |    |      |
|      | I    | new bitwise  |                  |   | e |    |      |
|      | want | primitives.* |                  |   | n |    |      |
|      | the  |              |                  |   | d |    |      |
|      | Node | *New Plutus  |                  |   | i |    |      |
|      | to   | V3 cost      |                  |   | n |    |      |
|      | sup  | model is     |                  |   | g |    |      |
|      | port | used         |                  |   |   |    |      |
|      | Pl   | correctly    |                  |   |   |    |      |
|      | utus | for the new  |                  |   |   |    |      |
|      | V3   | primitives.* |                  |   |   |    |      |
|      | requ |              |                  |   |   |    |      |
|      | irem | *Plutus      |                  |   |   |    |      |
|      | ents | scripts are  |                  |   |   |    |      |
|      | for  | correctly    |                  |   |   |    |      |
|      | CI   | used for     |                  |   |   |    |      |
|      | P-16 | DRep         |                  |   |   |    |      |
|      | 94** | voting.*     |                  |   |   |    |      |
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
| CH.A | **Le | This is a    | Detail pending   |   |   | A  | U    |
| PI11 | dger | placeholder  |                  |   |   | PI | PDAT |
|      | API  |              |                  |   |   | /C | E/RE |
|      | User |              |                  |   |   | LI | MOVE |
|      | Sto  |              |                  |   |   |    |      |
|      | ry** |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| VO16 | *    |              |                  |   |   | A  | U    |
|      | *SPO |              |                  |   |   | PI | PDAT |
|      | I    |              |                  |   |   | /C | E/RE |
|      | nter |              |                  |   |   | LI | MOVE |
|      | face |              |                  |   |   |    |      |
|      | User |              |                  |   |   |    |      |
|      | Sto  |              |                  |   |   |    |      |
|      | ry** |              |                  |   |   |    |      |
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
| *I   | *As  | **Timely**   |                  |   |   |    |      |
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
|      |      | **Correctly  |                  |   |   |    |      |
|      |      | according to |                  |   |   |    |      |
|      |      | CIP-1694     |                  |   |   |    |      |
|      |      | rules:       |                  |   |   |    |      |
|      |      | ***Parameter |                  |   |   |    |      |
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
| **SY |      |              |                  |   |   |    |      |
| STEM |      |              |                  |   |   |    |      |
| L    |      |              |                  |   |   |    |      |
| EVEL |      |              |                  |   |   |    |      |
| (not |      |              |                  |   |   |    |      |
| f    |      |              |                  |   |   |    |      |
| ully |      |              |                  |   |   |    |      |
| c    |      |              |                  |   |   |    |      |
| ompl |      |              |                  |   |   |    |      |
| eted |      |              |                  |   |   |    |      |
| ye   |      |              |                  |   |   |    |      |
| t)** |      |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| [[C  | **   | Hash value   | Given that I     |   | * | CI |      |
| IP1] | As** | of the       | access a Cardano |   | * | P- |      |
| {.un | any  | off-chain    | Explorer and     |   | D | 16 |      |
| derl | per  | Constitution | that it display  |   | e | 94 |      |
| ine} | sona | is recorded  | the ledger       |   | t |    |      |
| ](ht |      | on-chain     | states           |   | a | [* |      |
| tps: | **I  |              | accurately, Then |   | i | *[ |      |
| //do | wa   |              | I can access a   |   | l | L9 |      |
| cs.g | nt** |              | map of the       |   | P | 58 |      |
| oogl | the  |              | current          |   | e | ]{ |      |
| e.co | hash |              | constitution     |   | n | .u |      |
| m/do | v    |              | hash and the URL |   | d | nd |      |
| cume | alue |              | of the off-chain |   | i | er |      |
| nt/d | of   |              | document         |   | n | li |      |
| /1Ym | the  |              |                  |   | g | ne |      |
| j_Fo | o    |              |                  |   | * | }* |      |
| h3lV | ff-c |              |                  |   | * | *] |      |
| Yq2a | hain |              |                  |   |   | (h |      |
| sI5W | Cons |              |                  |   |   | tt |      |
| EdQY | titu |              |                  |   |   | ps |      |
| Bud5 | tion |              |                  |   |   | :/ |      |
| B8Kb | to   |              |                  |   |   | /g |      |
| Jcw4 | be   |              |                  |   |   | it |      |
| jpUw | reco |              |                  |   |   | hu |      |
| uv5p | rded |              |                  |   |   | b. |      |
| 8/ed | on-c |              |                  |   |   | co |      |
| it#b | hain |              |                  |   |   | m/ |      |
| ookm |      |              |                  |   |   | ca |      |
| ark= | **So |              |                  |   |   | rd |      |
| id.y | th   |              |                  |   |   | an |      |
| zo1a | at** |              |                  |   |   | o- |      |
| ziuw | I    |              |                  |   |   | fo |      |
| sxs) | can  |              |                  |   |   | un |      |
|      | ve   |              |                  |   |   | da |      |
|      | rify |              |                  |   |   | ti |      |
|      | the  |              |                  |   |   | on |      |
|      | auth |              |                  |   |   | /C |      |
|      | enti |              |                  |   |   | IP |      |
|      | city |              |                  |   |   | s/ |      |
|      | of   |              |                  |   |   | bl |      |
|      | the  |              |                  |   |   | ob |      |
|      | o    |              |                  |   |   | /d |      |
|      | ff-c |              |                  |   |   | e7 |      |
|      | hain |              |                  |   |   | 61 |      |
|      | docu |              |                  |   |   | 20 |      |
|      | ment |              |                  |   |   | a3 |      |
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
| [[C  | **   | Committee    | Given that the   |   | * | CI |      |
| IP2] | As** | members key  | node is up to    |   | * | P- |      |
| {.un | an   | hashes must  | date, then it    |   | D | 16 |      |
| derl | ada  | be recorded  | should include a |   | e | 94 |      |
| ine} | ho   | on chain and | record for each  |   | t |    |      |
| ](ht | lder | be publicly  | committee member |   | a | [* |      |
| tps: |      | accessible   | detailing their  |   | i | *[ |      |
| //do | **I  |              | key-hashes, term |   | l | L9 |      |
| cs.g | wa   | ADA holder   | information (end |   | P | 93 |      |
| oogl | nt** | must be able | epochs), and the |   | e | ]{ |      |
| e.co | the  | to check     | corresponding    |   | n | .u |      |
| m/do | key  | that the key | cold to hot key  |   | d | nd |      |
| cume | hash | hashes of    | authorization    |   | i | er |      |
| nt/d | of   | active and   | maps.            |   | n | li |      |
| /1Ym | ac   | expired      |                  |   | g | ne |      |
| j_Fo | tive | committee    |                  |   | * | }* |      |
| h3lV | and  | members are  |                  |   | * | *] |      |
| Yq2a | exp  | registered   |                  |   |   | (h |      |
| sI5W | ired | on-chain     |                  |   |   | tt |      |
| EdQY | C    | status       |                  |   |   | ps |      |
| Bud5 | ommi |              |                  |   |   | :/ |      |
| B8Kb | ttee |              |                  |   |   | /g |      |
| Jcw4 | Mem  |              |                  |   |   | it |      |
| jpUw | bers |              |                  |   |   | hu |      |
| uv5p | and  |              |                  |   |   | b. |      |
| 8/ed | t    |              |                  |   |   | co |      |
| it#b | heir |              |                  |   |   | m/ |      |
| ookm | t    |              |                  |   |   | ca |      |
| ark= | erms |              |                  |   |   | rd |      |
| id.e | to   |              |                  |   |   | an |      |
| lqu6 | be   |              |                  |   |   | o- |      |
| qa8l | re   |              |                  |   |   | fo |      |
| tse) | gist |              |                  |   |   | un |      |
|      | ered |              |                  |   |   | da |      |
|      | on-c |              |                  |   |   | ti |      |
|      | hain |              |                  |   |   | on |      |
|      |      |              |                  |   |   | /C |      |
|      | **So |              |                  |   |   | IP |      |
|      | th   |              |                  |   |   | s/ |      |
|      | at** |              |                  |   |   | bl |      |
|      | the  |              |                  |   |   | ob |      |
|      | sy   |              |                  |   |   | /d |      |
|      | stem |              |                  |   |   | e7 |      |
|      | can  |              |                  |   |   | 61 |      |
|      | c    |              |                  |   |   | 20 |      |
|      | ount |              |                  |   |   | a3 |      |
|      | t    |              |                  |   |   | 05 |      |
|      | heir |              |                  |   |   | 52 |      |
|      | v    |              |                  |   |   | ef |      |
|      | otes |              |                  |   |   | 62 |      |
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
| [[C  | **As | It must be   | Any ada holder   |   | * | CI |      |
| IP3] | an** | possible to  | can submit a     |   | * | P- |      |
| {.un | ada  | replace the  | governance       |   | D | 16 |      |
| derl | ho   | co           | action that      |   | e | 94 |      |
| ine} | lder | nstitutional | proposes to add  |   | t |    |      |
| ](ht |      | committee    | or remove one or |   | a | [* |      |
| tps: | **I  | via a        | many new         |   | i | *[ |      |
| //do | wa   | governance   | committee        |   | l | L9 |      |
| cs.g | nt** | action       | members.         |   | P | 97 |      |
| oogl | to   |              |                  |   | e | ]{ |      |
| e.co | be   |              | Given that a     |   | n | .u |      |
| m/do | able |              | governance       |   | d | nd |      |
| cume | to   |              | action to update |   | i | er |      |
| nt/d | su   |              | the committee    |   | n | li |      |
| /1Ym | bmit |              | has been         |   | g | ne |      |
| j_Fo | a    |              | proposed And     |   | * | }* |      |
| h3lV | prop |              | both SPO and     |   | * | *] |      |
| Yq2a | osal |              | DRep YES votes   |   |   | (h |      |
| sI5W | to   |              | are equal or     |   |   | tt |      |
| EdQY | rep  |              | greater than the |   |   | ps |      |
| Bud5 | lace |              | required         |   |   | :/ |      |
| B8Kb | all  |              | threshold        |   |   | /g |      |
| Jcw4 | or   |              | (depending on    |   |   | it |      |
| jpUw | part |              | state of         |   |   | hu |      |
| uv5p | of   |              | no-confidence or |   |   | b. |      |
| 8/ed | the  |              | normal state)    |   |   | co |      |
| it#b | cur  |              |                  |   |   | m/ |      |
| ookm | rent |              | The governance   |   |   | ca |      |
| ark= | co   |              | action is        |   |   | rd |      |
| id.p | nsti |              | ratified and     |   |   | an |      |
| ddqk | tuti |              | enacted          |   |   | o- |      |
| syfs | onal |              | automatically at |   |   | fo |      |
| hgc) | c    |              | the next epoch   |   |   | un |      |
|      | ommi |              | transition,      |   |   | da |      |
|      | ttee |              | otherwise it's   |   |   | ti |      |
|      |      |              | expired.         |   |   | on |      |
|      | **So |              |                  |   |   | /C |      |
|      | th   |              |                  |   |   | IP |      |
|      | at** |              |                  |   |   | s/ |      |
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
| [[C  | **As | Size of the  | **Detail         |   | * | [* |      |
| IP4] | an** | co           | Pending**        |   | * | *[ |      |
| {.un | ada  | nstitutional |                  |   | D | L1 |      |
| derl | ho   | committee    |                  |   | e | 00 |      |
| ine} | lder | must be      |                  |   | t | 9] |      |
| ](ht |      | variable     |                  |   | a | {. |      |
| tps: | I    |              |                  |   | i | un |      |
| //do | want |              |                  |   | l | de |      |
| cs.g | the  |              |                  |   | P | rl |      |
| oogl | size |              |                  |   | e | in |      |
| e.co | of   |              |                  |   | n | e} |      |
| m/do | the  |              |                  |   | d | ** |      |
| cume | co   |              |                  |   | i | ]( |      |
| nt/d | nsti |              |                  |   | n | ht |      |
| /1Ym | tuti |              |                  |   | g | tp |      |
| j_Fo | onal |              |                  |   | * | s: |      |
| h3lV | c    |              |                  |   | * | // |      |
| Yq2a | ommi |              |                  |   |   | gi |      |
| sI5W | ttee |              |                  |   |   | th |      |
| EdQY |      |              |                  |   |   | ub |      |
| Bud5 | To   |              |                  |   |   | .c |      |
| B8Kb | be   |              |                  |   |   | om |      |
| Jcw4 | n    |              |                  |   |   | /c |      |
| jpUw | ot-f |              |                  |   |   | ar |      |
| uv5p | ixed |              |                  |   |   | da |      |
| 8/ed |      |              |                  |   |   | no |      |
| it#b | So   |              |                  |   |   | -f |      |
| ookm | that |              |                  |   |   | ou |      |
| ark= | I    |              |                  |   |   | nd |      |
| id.m | can  |              |                  |   |   | at |      |
| ca6c | pro  |              |                  |   |   | io |      |
| vcoh | pose |              |                  |   |   | n/ |      |
| t53) | a    |              |                  |   |   | CI |      |
|      | d    |              |                  |   |   | Ps |      |
|      | iffe |              |                  |   |   | /b |      |
|      | rent |              |                  |   |   | lo |      |
|      | size |              |                  |   |   | b/ |      |
|      | via  |              |                  |   |   | ad |      |
|      | a    |              |                  |   |   | a2 |      |
|      | go   |              |                  |   |   | cf |      |
|      | vern |              |                  |   |   | 6a |      |
|      | ance |              |                  |   |   | 9e |      |
|      | ac   |              |                  |   |   | 27 |      |
|      | tion |              |                  |   |   | fb |      |
|      |      |              |                  |   |   | df |      |
|      |      |              |                  |   |   | 37 |      |
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
| [[C  | As   | **Size of**  | **Detail         |   | * | [* |      |
| IP5] | an   | committee    | Pending**        |   | * | *[ |      |
| {.un | ada  | threshold    |                  |   | D | L1 |      |
| derl | hol  | must be      |                  |   | e | 01 |      |
| ine} | der, | variable     |                  |   | t | 1] |      |
| ](ht |      |              |                  |   | a | {. |      |
| tps: | I    |              |                  |   | i | un |      |
| //do | want |              |                  |   | l | de |      |
| cs.g | that |              |                  |   | P | rl |      |
| oogl | the  |              |                  |   | e | in |      |
| e.co | c    |              |                  |   | n | e} |      |
| m/do | ommi |              |                  |   | d | ** |      |
| cume | ttee |              |                  |   | i | ]( |      |
| nt/d | t    |              |                  |   | n | ht |      |
| /1Ym | hres |              |                  |   | g | tp |      |
| j_Fo | hold |              |                  |   | * | s: |      |
| h3lV | (the |              |                  |   | * | // |      |
| Yq2a | frac |              |                  |   |   | gi |      |
| sI5W | tion |              |                  |   |   | th |      |
| EdQY | of   |              |                  |   |   | ub |      |
| Bud5 | c    |              |                  |   |   | .c |      |
| B8Kb | ommi |              |                  |   |   | om |      |
| Jcw4 | ttee |              |                  |   |   | /c |      |
| jpUw | is   |              |                  |   |   | ar |      |
| uv5p | not  |              |                  |   |   | da |      |
| 8/ed | f    |              |                  |   |   | no |      |
| it#b | ixed |              |                  |   |   | -f |      |
| ookm |      |              |                  |   |   | ou |      |
| ark= | So   |              |                  |   |   | nd |      |
| id.t | that |              |                  |   |   | at |      |
| dyxk | I    |              |                  |   |   | io |      |
| 950f | can  |              |                  |   |   | n/ |      |
| 5v8) | pro  |              |                  |   |   | CI |      |
|      | pose |              |                  |   |   | Ps |      |
|      | a    |              |                  |   |   | /b |      |
|      | d    |              |                  |   |   | lo |      |
|      | iffe |              |                  |   |   | b/ |      |
|      | rent |              |                  |   |   | ad |      |
|      | t    |              |                  |   |   | a2 |      |
|      | hres |              |                  |   |   | cf |      |
|      | hold |              |                  |   |   | 6a |      |
|      | via  |              |                  |   |   | 9e |      |
|      | a    |              |                  |   |   | 27 |      |
|      | go   |              |                  |   |   | fb |      |
|      | vern |              |                  |   |   | df |      |
|      | ance |              |                  |   |   | 37 |      |
|      | ac   |              |                  |   |   | ca |      |
|      | tion |              |                  |   |   | 1b |      |
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
|      |      |              |                  |   |   | 01 |      |
|      |      |              |                  |   |   | 1) |      |
+------+------+--------------+------------------+---+---+----+------+
| CIP6 | As   | Users must   | **Detail         |   | * | [* |      |
|      | an   | be able to   | Pending**        |   | * | *[ |      |
|      | ada  | elect an     |                  |   | D | L1 |      |
|      | ho   | empty        |                  |   | e | 01 |      |
|      | lder | committee    |                  |   | t | 4] |      |
|      |      |              |                  |   | a | {. |      |
|      | I    | Ratifying    |                  |   | i | un |      |
|      | want | governance   |                  |   | l | de |      |
|      | to   | actions must |                  |   | P | rl |      |
|      | be   | be possible  |                  |   | e | in |      |
|      | able | without      |                  |   | n | e} |      |
|      | to   | co           |                  |   | d | ** |      |
|      | have | nstitutional |                  |   | i | ]( |      |
|      | e    | committee    |                  |   | n | ht |      |
|      | lect |              |                  |   | g | tp |      |
|      | an   |              |                  |   | * | s: |      |
|      | e    |              |                  |   | * | // |      |
|      | mpty |              |                  |   |   | gi |      |
|      | c    |              |                  |   |   | th |      |
|      | ommi |              |                  |   |   | ub |      |
|      | ttee |              |                  |   |   | .c |      |
|      | if   |              |                  |   |   | om |      |
|      | the  |              |                  |   |   | /c |      |
|      | c    |              |                  |   |   | ar |      |
|      | ommu |              |                  |   |   | da |      |
|      | nity |              |                  |   |   | no |      |
|      | wi   |              |                  |   |   | -f |      |
|      | shes |              |                  |   |   | ou |      |
|      | to   |              |                  |   |   | nd |      |
|      | abo  |              |                  |   |   | at |      |
|      | lish |              |                  |   |   | io |      |
|      | the  |              |                  |   |   | n/ |      |
|      | co   |              |                  |   |   | CI |      |
|      | nsti |              |                  |   |   | Ps |      |
|      | tuti |              |                  |   |   | /b |      |
|      | onal |              |                  |   |   | lo |      |
|      | c    |              |                  |   |   | b/ |      |
|      | ommi |              |                  |   |   | ad |      |
|      | ttee |              |                  |   |   | a2 |      |
|      | enti |              |                  |   |   | cf |      |
|      | rely |              |                  |   |   | 6a |      |
|      |      |              |                  |   |   | 9e |      |
|      | So   |              |                  |   |   | 27 |      |
|      | that |              |                  |   |   | fb |      |
|      | SPO  |              |                  |   |   | df |      |
|      | and  |              |                  |   |   | 37 |      |
|      | D    |              |                  |   |   | ca |      |
|      | reps |              |                  |   |   | 1b |      |
|      | can  |              |                  |   |   | e0 |      |
|      | cont |              |                  |   |   | 78 |      |
|      | inue |              |                  |   |   | 03 |      |
|      | to   |              |                  |   |   | 71 |      |
|      | ra   |              |                  |   |   | fb |      |
|      | tify |              |                  |   |   | ab |      |
|      | go   |              |                  |   |   | 2b |      |
|      | vern |              |                  |   |   | 77 |      |
|      | ance |              |                  |   |   | 48 |      |
|      | act  |              |                  |   |   | /C |      |
|      | ions |              |                  |   |   | IP |      |
|      | wit  |              |                  |   |   | -1 |      |
|      | hout |              |                  |   |   | 69 |      |
|      | the  |              |                  |   |   | 4/ |      |
|      | need |              |                  |   |   | RE |      |
|      | of a |              |                  |   |   | AD |      |
|      | co   |              |                  |   |   | ME |      |
|      | nsti |              |                  |   |   | .m |      |
|      | tuti |              |                  |   |   | d? |      |
|      | onal |              |                  |   |   | pl |      |
|      | c    |              |                  |   |   | ai |      |
|      | ommi |              |                  |   |   | n= |      |
|      | ttee |              |                  |   |   | 1# |      |
|      |      |              |                  |   |   | L1 |      |
|      |      |              |                  |   |   | 01 |      |
|      |      |              |                  |   |   | 4) |      |
+------+------+--------------+------------------+---+---+----+------+
| CIP7 | **   | **There must | **Detail         |   | * | CI |      |
|      | As** | be a command | Pending**        |   | * | P- |      |
|      | an   | in in the    |                  |   | D | 16 |      |
|      | Ada  | Cardano CLI  |                  |   | e | 94 |      |
|      | hol  | allowing the |                  |   | t |    |      |
|      | der, | user to      |                  |   | a |    |      |
|      |      | submit a     |                  |   | i |    |      |
|      | **I  | governance   |                  |   | l |    |      |
|      | wa   | action**     |                  |   | P |    |      |
|      | nt** |              |                  |   | e |    |      |
|      | to   | The input    |                  |   | n |    |      |
|      | su   | must include |                  |   | d |    |      |
|      | bmit | validation   |                  |   | i |    |      |
|      | a    | checks for   |                  |   | n |    |      |
|      | go   | format and   |                  |   | g |    |      |
|      | vern | criteria     |                  |   | * |    |      |
|      | ance |              |                  |   | * |    |      |
|      | act  | After        |                  |   |   |    |      |
|      | ion, | successful   |                  |   |   |    |      |
|      |      | validation   |                  |   |   |    |      |
|      | **So | the          |                  |   |   |    |      |
|      | th   |              |                  |   |   |    |      |
|      | at** | user must be |                  |   |   |    |      |
|      | it   | informed of  |                  |   |   |    |      |
|      | can  | confirmation |                  |   |   |    |      |
|      | be   | through the  |                  |   |   |    |      |
|      | co   | CLI          |                  |   |   |    |      |
|      | nsid |              |                  |   |   |    |      |
|      | ered | An action    |                  |   |   |    |      |
|      | by   | should have  |                  |   |   |    |      |
|      | the  | an accepted  |                  |   |   |    |      |
|      | go   | or rejected  |                  |   |   |    |      |
|      | vern | status?      |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | bod  |              |                  |   |   |    |      |
|      | ies/ |              |                  |   |   |    |      |
|      | proc |              |                  |   |   |    |      |
|      | ess. |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CIP8 | **   | DReps must   | Given that a     |   | * | CI |      |
|      | As** | have access  | Drep has casted  |   | * | P- |      |
|      | a    | to the list  | a vote the       |   | D | 16 |      |
|      | dele | of current   | system           |   | e | 94 |      |
|      | gate | governance   | accurately       |   | t |    |      |
|      | re   | actions (can | records and      |   | a |    |      |
|      | pres | we specify   | reflects these   |   | i |    |      |
|      | enta | where they   | votes.           |   | l |    |      |
|      | tive | get it?).    |                  |   | P |    |      |
|      | (DR  |              |                  |   | e |    |      |
|      | ep), | DReps should |                  |   | n |    |      |
|      |      | be able to   |                  |   | d |    |      |
|      | **I  | cast their   |                  |   | i |    |      |
|      | wa   | vote on each |                  |   | n |    |      |
|      | nt** | action       |                  |   | g |    |      |
|      | to   | (through the |                  |   | * |    |      |
|      | vote | CL or        |                  |   | * |    |      |
|      | on   | through an   |                  |   |   |    |      |
|      | s    | app)?        |                  |   |   |    |      |
|      | ubmi |              |                  |   |   |    |      |
|      | tted | An action    |                  |   |   |    |      |
|      | go   | should have  |                  |   |   |    |      |
|      | vern | an accepted  |                  |   |   |    |      |
|      | ance | or rejected  |                  |   |   |    |      |
|      | acti | status?      |                  |   |   |    |      |
|      | ons, |              |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | **So |              |                  |   |   |    |      |
|      | th   |              |                  |   |   |    |      |
|      | at** |              |                  |   |   |    |      |
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
| CIP9 | **   | Users must   | **Detail         |   | * | CI |      |
|      | As** | be able to   | Pending**        |   | * | P- |      |
|      | an   | view a list  |                  |   | D | 16 |      |
|      | Ada  | of           |                  |   | e | 94 |      |
|      | hol  | governance   |                  |   | t |    |      |
|      | der, | actions with |                  |   | a |    |      |
|      |      | their        |                  |   | i |    |      |
|      | **I  | current      |                  |   | l |    |      |
|      | wa   | status.      |                  |   | P |    |      |
|      | nt** |              |                  |   | e |    |      |
|      | to   | The status   |                  |   | n |    |      |
|      | view | must include |                  |   | d |    |      |
|      | the  | stages like  |                  |   | i |    |      |
|      | st   | submission,  |                  |   | n |    |      |
|      | atus | voting,      |                  |   | g |    |      |
|      | of   | r            |                  |   | * |    |      |
|      | go   | atification, |                  |   | * |    |      |
|      | vern | timeline.    |                  |   |   |    |      |
|      | ance |              |                  |   |   |    |      |
|      | acti | The system   |                  |   |   |    |      |
|      | ons, | must provide |                  |   |   |    |      |
|      |      | real-time    |                  |   |   |    |      |
|      | **So | updates on   |                  |   |   |    |      |
|      | th   | the status.  |                  |   |   |    |      |
|      | at** |              |                  |   |   |    |      |
|      | I am |              |                  |   |   |    |      |
|      | info |              |                  |   |   |    |      |
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
| C    | **   | ADA holders  | **Detail         |   |   |    |      |
| IP10 | As** | can select a | Pending**        |   |   |    |      |
|      | an   | DRep to      |                  |   |   |    |      |
|      | Ada  | delegate     |                  |   |   |    |      |
|      | hol  | their voting |                  |   |   |    |      |
|      | der, | rights.      |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | **I  | The          |                  |   |   |    |      |
|      | wa   | delegation   |                  |   |   |    |      |
|      | nt** | process      |                  |   |   |    |      |
|      | to   | should be    |                  |   |   |    |      |
|      | dele | u            |                  |   |   |    |      |
|      | gate | ser-friendly |                  |   |   |    |      |
|      | my   | and must be  |                  |   |   |    |      |
|      | vo   | secure.      |                  |   |   |    |      |
|      | ting |              |                  |   |   |    |      |
|      | ri   | The system   |                  |   |   |    |      |
|      | ghts | must         |                  |   |   |    |      |
|      | to a | confirms     |                  |   |   |    |      |
|      | D    | successful   |                  |   |   |    |      |
|      | Rep, | delegation.  |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | **So |              |                  |   |   |    |      |
|      | th   |              |                  |   |   |    |      |
|      | at** |              |                  |   |   |    |      |
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
| C    | **   | SPOs must    | **Detail         |   |   |    |      |
| IP11 | As** | have access  | Pending**        |   |   |    |      |
|      | an   | to           |                  |   |   |    |      |
|      | SPO, | governance   |                  |   |   |    |      |
|      |      | actions for  |                  |   |   |    |      |
|      | **I  | voting.      |                  |   |   |    |      |
|      | wa   |              |                  |   |   |    |      |
|      | nt** | SPOs can     |                  |   |   |    |      |
|      | to   | cast their   |                  |   |   |    |      |
|      | par  | votes based  |                  |   |   |    |      |
|      | tici | on the ADA   |                  |   |   |    |      |
|      | pate | staked in    |                  |   |   |    |      |
|      | in   | their pools. |                  |   |   |    |      |
|      | the  |              |                  |   |   |    |      |
|      | go   | The system   |                  |   |   |    |      |
|      | vern | accurately   |                  |   |   |    |      |
|      | ance | reflects the |                  |   |   |    |      |
|      | vot  | votes of     |                  |   |   |    |      |
|      | ing, | SPOs.        |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      | **So |              |                  |   |   |    |      |
|      | th   |              |                  |   |   |    |      |
|      | at** |              |                  |   |   |    |      |
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
| *    |      |              |                  |   |   |    |      |
| *CAR |      |              |                  |   |   |    |      |
| DANO |      |              |                  |   |   |    |      |
| CLI  |      |              |                  |   |   |    |      |
| US** |      |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | **   | When I       | Given that a     |   |   | [[ |      |
| LI01 | As** | provide the  | holder provides  |   |   | L9 |      |
|      | an   | off-chain    | the offchain     |   |   | 58 |      |
|      | Ada  | text of the  | text of the      |   |   | ]{ |      |
|      | hol  | C            | constitution     |   |   | .u |      |
|      | der, | onstitution, | then cardo-cli   |   |   | nd |      |
|      |      | the          | should return    |   |   | er |      |
|      | **I  | cardano-cli  | the              |   |   | li |      |
|      | wa   | should       | corresponding    |   |   | ne |      |
|      | nt** | calculate    | blake2b-256 hash |   |   | }] |      |
|      | to   | and return   |                  |   |   | (h |      |
|      | ob   | the          | Given that it is |   |   | tt |      |
|      | tain | c            | the same         |   |   | ps |      |
|      | the  | orresponding | document, the    |   |   | :/ |      |
|      | hash | blake2b-256  | resulting hash   |   |   | /g |      |
|      | of   | hash of the  | should match the |   |   | it |      |
|      | the  | document.    | one registered   |   |   | hu |      |
|      | o    |              | on-chain.        |   |   | b. |      |
|      | ff-c |              |                  |   |   | co |      |
|      | hain |              |                  |   |   | m/ |      |
|      | text |              |                  |   |   | ca |      |
|      | of a |              |                  |   |   | rd |      |
|      | Cons |              |                  |   |   | an |      |
|      | titu |              |                  |   |   | o- |      |
|      | tion |              |                  |   |   | fo |      |
|      |      |              |                  |   |   | un |      |
|      | **So |              |                  |   |   | da |      |
|      | th   |              |                  |   |   | ti |      |
|      | at** |              |                  |   |   | on |      |
|      | I    |              |                  |   |   | /C |      |
|      | can  |              |                  |   |   | IP |      |
|      | com  |              |                  |   |   | s/ |      |
|      | pare |              |                  |   |   | bl |      |
|      | it   |              |                  |   |   | ob |      |
|      | aga  |              |                  |   |   | /d |      |
|      | inst |              |                  |   |   | 6c |      |
|      | the  |              |                  |   |   | 5a |      |
|      | hash |              |                  |   |   | d3 |      |
|      | re   |              |                  |   |   | a7 |      |
|      | gist |              |                  |   |   | 7b |      |
|      | ered |              |                  |   |   | 46 |      |
|      | on-c |              |                  |   |   | 84 |      |
|      | hain |              |                  |   |   | bc |      |
|      | to   |              |                  |   |   | 19 |      |
|      | ve   |              |                  |   |   | f3 |      |
|      | rify |              |                  |   |   | ca |      |
|      | its  |              |                  |   |   | fb |      |
|      | a    |              |                  |   |   | 75 |      |
|      | uthe |              |                  |   |   | b4 |      |
|      | ntic |              |                  |   |   | 88 |      |
|      | ity. |              |                  |   |   | 6a |      |
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
| C    | **   | When I       | Given that a     |   |   | [[ |      |
| LI02 | As** | provide the  | holder provides  |   |   | L9 |      |
|      | an   | off-chain    | the offchain     |   |   | 58 |      |
|      | Ada  | text of the  | text of the      |   |   | ]{ |      |
|      | hol  | C            | constitution     |   |   | .u |      |
|      | der, | onstitution, | then cardo-cli   |   |   | nd |      |
|      |      | the          | should return    |   |   | er |      |
|      | **I  | cardano-cli  | the              |   |   | li |      |
|      | wa   | should       | corresponding    |   |   | ne |      |
|      | nt** | calculate    | blake2b-256 hash |   |   | }] |      |
|      | to   | and return   |                  |   |   | (h |      |
|      | gene | the          | Given that it is |   |   | tt |      |
|      | rate | c            | the same         |   |   | ps |      |
|      | the  | orresponding | document, the    |   |   | :/ |      |
|      | hash | blake2b-256  | resulting hash   |   |   | /g |      |
|      | of   | hash of the  | should match the |   |   | it |      |
|      | the  | document.    | one registered   |   |   | hu |      |
|      | o    |              | on-chain.        |   |   | b. |      |
|      | ff-c |              |                  |   |   | co |      |
|      | hain |              |                  |   |   | m/ |      |
|      | text |              |                  |   |   | ca |      |
|      | for  |              |                  |   |   | rd |      |
|      | a    |              |                  |   |   | an |      |
|      | prop |              |                  |   |   | o- |      |
|      | osed |              |                  |   |   | fo |      |
|      | Cons |              |                  |   |   | un |      |
|      | titu |              |                  |   |   | da |      |
|      | tion |              |                  |   |   | ti |      |
|      |      |              |                  |   |   | on |      |
|      | **So |              |                  |   |   | /C |      |
|      | th   |              |                  |   |   | IP |      |
|      | at** |              |                  |   |   | s/ |      |
|      | the  |              |                  |   |   | bl |      |
|      | hash |              |                  |   |   | ob |      |
|      | can  |              |                  |   |   | /d |      |
|      | be   |              |                  |   |   | 6c |      |
|      | util |              |                  |   |   | 5a |      |
|      | ized |              |                  |   |   | d3 |      |
|      | in a |              |                  |   |   | a7 |      |
|      | go   |              |                  |   |   | 7b |      |
|      | vern |              |                  |   |   | 46 |      |
|      | ance |              |                  |   |   | 84 |      |
|      | act  |              |                  |   |   | bc |      |
|      | ion. |              |                  |   |   | 19 |      |
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
| C    | **   | [The feature | Typing           |   |   | [  |      |
| LI03 | As** | im           | [cardano-cli     |   |   | [L |      |
|      | a    | plementation | conway           |   |   | 96 |      |
|      | p    | should       | governance       |   |   | 6] |      |
|      | oten | include a    | committee        |   |   | {. |      |
|      | tial | new          | key-gen-cold     |   |   | un |      |
|      | Co   | command:\    | with accepted    |   |   | de |      |
|      | nsti | \            | input parameters |   |   | rl |      |
|      | tuti | cardano-cli  | generates a COLD |   |   | in |      |
|      | onal | conway       | key pair. If a   |   |   | e} |      |
|      | C    | governance   | parameter or the |   |   | ]( |      |
|      | ommi | committee    | command format   |   |   | ht |      |
|      | ttee | key-gen-     | is incorrect an  |   |   | tp |      |
|      | mem  | cold]{.mark} | error is         |   |   | s: |      |
|      | ber, |              | raised]{.mark}   |   |   | // |      |
|      |      |              |                  |   |   | gi |      |
|      | **I  |              |                  |   |   | th |      |
|      | wa   |              |                  |   |   | ub |      |
|      | nt** |              |                  |   |   | .c |      |
|      | to   |              |                  |   |   | om |      |
|      | gene |              |                  |   |   | /c |      |
|      | rate |              |                  |   |   | ar |      |
|      | COLD |              |                  |   |   | da |      |
|      | key  |              |                  |   |   | no |      |
|      | pair |              |                  |   |   | -f |      |
|      |      |              |                  |   |   | ou |      |
|      | **So |              |                  |   |   | nd |      |
|      | th   |              |                  |   |   | at |      |
|      | at** |              |                  |   |   | io |      |
|      | I    |              |                  |   |   | n/ |      |
|      | can  |              |                  |   |   | CI |      |
|      | be   |              |                  |   |   | Ps |      |
|      | prop |              |                  |   |   | /b |      |
|      | osed |              |                  |   |   | lo |      |
|      | for  |              |                  |   |   | b/ |      |
|      | the  |              |                  |   |   | d6 |      |
|      | C    |              |                  |   |   | c5 |      |
|      | ommi |              |                  |   |   | ad |      |
|      | ttee |              |                  |   |   | 3a |      |
|      | in a |              |                  |   |   | 77 |      |
|      | Go   |              |                  |   |   | b4 |      |
|      | vern |              |                  |   |   | 68 |      |
|      | ance |              |                  |   |   | 4b |      |
|      | ac   |              |                  |   |   | c1 |      |
|      | tion |              |                  |   |   | 9f |      |
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
|      |      | va           | [**Type**        |   |   | in |      |
|      |      | lue.]{.mark} | \"Constit        |   |   | e} |      |
|      |      |              | utionalCommittee |   |   | ]( |      |
|      |      | [**Type**    | ColdSigningKey_e |   |   | ht |      |
|      |      | \"Constit    | d25519\"]{.mark} |   |   | tp |      |
|      |      | utionalCommi |                  |   |   | s: |      |
|      |      | tteeColdSign | **[Descr         |   |   | // |      |
|      |      | ingKey_ed255 | iption]{.mark}** |   |   | gi |      |
|      |      | 19\"]{.mark} |                  |   |   | th |      |
|      |      |              | [                |   |   | ub |      |
|      |      | **[Descripti | \"Constitutional |   |   | .c |      |
|      |      | on]{.mark}** | Committee Cold   |   |   | om |      |
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
|      |      | **Type**     | fields are:      |   |   | de |      |
|      |      | \"CCons      |                  |   |   | rl |      |
|      |      | titutionalCo | **Type**         |   |   | in |      |
|      |      | mmitteeColdV | [\"CConstitution |   |   | e} |      |
|      |      | erificationK | alCommitteeColdV |   |   | ]( |      |
|      |      | ey_ed25519\" | erificationKey_e |   |   | ht |      |
|      |      |              | d25519\"]{.mark} |   |   | tp |      |
|      |      | **D          |                  |   |   | s: |      |
|      |      | escription** | **Description**  |   |   | // |      |
|      |      |              |                  |   |   | gi |      |
|      |      | \"Co         | [                |   |   | th |      |
|      |      | nstitutional | \"Constitutional |   |   | ub |      |
|      |      | Committee    | Committee Cold   |   |   | .c |      |
|      |      | Cold         | Verification     |   |   | om |      |
|      |      | Verification | Key\"]{.mark}    |   |   | /c |      |
|      |      | Key\"        |                  |   |   | ar |      |
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
|      |      | Failing to   | **Given** the    |   |   | [  |      |
|      |      | provide a    | user has not     |   |   | [L |      |
|      |      | file name    | inputed either   |   |   | 96 |      |
|      |      | for any of   | [\--co           |   |   | 6] |      |
|      |      |              | ld-verification- |   |   | {. |      |
|      |      | \--co        | key-file]{.mark} |   |   | un |      |
|      |      | ld-verificat | OR               |   |   | de |      |
|      |      | ion-key-file |                  |   |   | rl |      |
|      |      |              | [                |   |   | in |      |
|      |      | \--cold-sign | \--cold-signing- |   |   | e} |      |
|      |      | ing-key-file | key-file]{.mark} |   |   | ]( |      |
|      |      |              | parameters       |   |   | ht |      |
|      |      | fails with   | **THEN** the     |   |   | tp |      |
|      |      | an           | command fails    |   |   | s: |      |
|      |      | appropriate  | and returns an   |   |   | // |      |
|      |      | error        | error to the     |   |   | gi |      |
|      |      | message.     | users informing  |   |   | th |      |
|      |      |              | them to fill     |   |   | ub |      |
|      |      |              | those parameters |   |   | .c |      |
|      |      |              | in. The error    |   |   | om |      |
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
| C    | **   | [The feature | Given that a     |   |   | [  |      |
| LI04 | As** | im           | potential        |   |   | [L |      |
|      | p    | plementation | constitutional   |   |   | 96 |      |
|      | oten | should       | committee member |   |   | 6] |      |
|      | tial | include a    | has entered the  |   |   | {. |      |
|      | Co   | new          | [cardano-cli     |   |   | un |      |
|      | nsti | command:\    | conway           |   |   | de |      |
|      | tuti | \            | governance       |   |   | rl |      |
|      | onal | cardano-cli  | committee        |   |   | in |      |
|      | C    | conway       | key-gen-hot      |   |   | e} |      |
|      | ommi | governance   | command with all |   |   | ]( |      |
|      | ttee | committee    | the required and |   |   | ht |      |
|      | mem  | key-gen      | correct          |   |   | tp |      |
|      | ber, | -hot]{.mark} | pa               |   |   | s: |      |
|      |      |              | rameters]{.mark} |   |   | // |      |
|      | **I  |              | then the command |   |   | gi |      |
|      | wa   |              | is executed      |   |   | th |      |
|      | nt** |              | successfully and |   |   | ub |      |
|      | to   |              | a HOT key pair   |   |   | .c |      |
|      | gene |              | is generated.    |   |   | om |      |
|      | rate |              |                  |   |   | /c |      |
|      | HOT  |              | [If a parameter  |   |   | ar |      |
|      | key  |              | or the command   |   |   | da |      |
|      | pair |              | format is        |   |   | no |      |
|      |      |              | incorrect an     |   |   | -f |      |
|      | **So |              | error is         |   |   | ou |      |
|      | th   |              | raised]{.mark}   |   |   | nd |      |
|      | at** |              |                  |   |   | at |      |
|      | I    |              |                  |   |   | io |      |
|      | can  |              |                  |   |   | n/ |      |
|      | a    |              |                  |   |   | CI |      |
|      | utho |              |                  |   |   | Ps |      |
|      | rise |              |                  |   |   | /b |      |
|      | the  |              |                  |   |   | lo |      |
|      | Hot  |              |                  |   |   | b/ |      |
|      | key  |              |                  |   |   | d6 |      |
|      | to   |              |                  |   |   | c5 |      |
|      | sign |              |                  |   |   | ad |      |
|      | v    |              |                  |   |   | 3a |      |
|      | otes |              |                  |   |   | 77 |      |
|      | on   |              |                  |   |   | b4 |      |
|      | be   |              |                  |   |   | 68 |      |
|      | half |              |                  |   |   | 4b |      |
|      | of   |              |                  |   |   | c1 |      |
|      | the  |              |                  |   |   | 9f |      |
|      | Cold |              |                  |   |   | 3c |      |
|      | key  |              |                  |   |   | af |      |
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
|      |      | Includes a   | Typing           |   | * | [  |      |
|      |      | c            | [cardano-cli     |   | * | [L |      |
|      |      | orresponding | conway           |   | D | 96 |      |
|      |      | CLI usage    | governance       |   | e | 6] |      |
|      |      | describing   | committee        |   | t | {. |      |
|      |      | the feature, | key-gen-hot      |   | a | un |      |
|      |      | how to use   | displays command |   | i | de |      |
|      |      | it and the   | usage]{.mark}    |   | l | rl |      |
|      |      | types of the |                  |   | P | in |      |
|      |      | inputs and   |                  |   | e | e} |      |
|      |      | outputs.     |                  |   | n | ]( |      |
|      |      |              |                  |   | d | ht |      |
|      |      |              |                  |   | i | tp |      |
|      |      |              |                  |   | n | s: |      |
|      |      |              |                  |   | g | // |      |
|      |      |              |                  |   | * | gi |      |
|      |      |              |                  |   | * | th |      |
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
|      |      | The command  | Both flags are   |   | * | [  |      |
|      |      | must accept  | mandatory and    |   | * | [L |      |
|      |      | two flags    | each produces    |   | D | 96 |      |
|      |      |              | the              |   | e | 6] |      |
|      |      | \--verificat | corresponding    |   | t | {. |      |
|      |      | ion-key-file | verification or  |   | a | un |      |
|      |      |              | signing key file |   | i | de |      |
|      |      | \--sign      |                  |   | l | rl |      |
|      |      | ing-key-file |                  |   | P | in |      |
|      |      |              |                  |   | e | e} |      |
|      |      |              |                  |   | n | ]( |      |
|      |      |              |                  |   | d | ht |      |
|      |      |              |                  |   | i | tp |      |
|      |      |              |                  |   | n | s: |      |
|      |      |              |                  |   | g | // |      |
|      |      |              |                  |   | * | gi |      |
|      |      |              |                  |   | * | th |      |
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
|      |      | [The         | Given that the   |   |   | [  |      |
|      |      | **signing**  | signing key is   |   |   | [L |      |
|      |      | key text     | saved on a text  |   |   | 96 |      |
|      |      | envelope     | envelope format, |   |   | 6] |      |
|      |      | contains the | the type and     |   |   | {. |      |
|      |      | correct      | description      |   |   | un |      |
|      |      | type,        | fields are:      |   |   | de |      |
|      |      | description, |                  |   |   | rl |      |
|      |      | and CBOR     | *                |   |   | in |      |
|      |      | va           | *[Type]{.mark}** |   |   | e} |      |
|      |      | lue.]{.mark} | \                |   |   | ]( |      |
|      |      |              | "ConstitutionalC |   |   | ht |      |
|      |      | [**Type**    | ommitteeColdSign |   |   | tp |      |
|      |      | \"Constit    | ingKey_ed25519\" |   |   | s: |      |
|      |      | utionalCommi |                  |   |   | // |      |
|      |      | tteeColdSign | **[Descr         |   |   | gi |      |
|      |      | ingKey_ed255 | iption]{.mark}** |   |   | th |      |
|      |      | 19\"]{.mark} |                  |   |   | ub |      |
|      |      |              | \"Constitutional |   |   | .c |      |
|      |      | **[Descripti | Committee Cold   |   |   | om |      |
|      |      | on]{.mark}** | Signing Key\"    |   |   | /c |      |
|      |      |              |                  |   |   | ar |      |
|      |      | [\"Co        |                  |   |   | da |      |
|      |      | nstitutional |                  |   |   | no |      |
|      |      | Committee    |                  |   |   | -f |      |
|      |      | Cold Signing |                  |   |   | ou |      |
|      |      | K            |                  |   |   | nd |      |
|      |      | ey\"]{.mark} |                  |   |   | at |      |
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
|      |      | **ve         | verification key |   |   | [L |      |
|      |      | rification** | is saved on a    |   |   | 96 |      |
|      |      | key text     | text envelope    |   |   | 6] |      |
|      |      | envelope     | format, the type |   |   | {. |      |
|      |      | has:         | and description  |   |   | un |      |
|      |      |              | fields are:      |   |   | de |      |
|      |      | **Type\      |                  |   |   | rl |      |
|      |      | **\"CCons    | **Type\          |   |   | in |      |
|      |      | titutionalCo | **\"CCons        |   |   | e} |      |
|      |      | mmitteeColdV | titutionalCommit |   |   | ]( |      |
|      |      | erificationK | teeColdVerificat |   |   | ht |      |
|      |      | ey_ed25519\" | ionKey_ed25519\" |   |   | tp |      |
|      |      |              |                  |   |   | s: |      |
|      |      | **           | **Description\   |   |   | // |      |
|      |      | Description\ | **               |   |   | gi |      |
|      |      | **\"Co       | \"Constitutional |   |   | th |      |
|      |      | nstitutional | Committee Cold   |   |   | ub |      |
|      |      | Committee    | Verification     |   |   | .c |      |
|      |      | Cold         | Key\"            |   |   | om |      |
|      |      | Verification |                  |   |   | /c |      |
|      |      | Key\"        |                  |   |   | ar |      |
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
|      |      | Failing to   | **Given** the    |   |   | [  |      |
|      |      | provide a    | user has not     |   |   | [L |      |
|      |      | file name    | inputted either  |   |   | 96 |      |
|      |      | for any of   | \--verif         |   |   | 6] |      |
|      |      | the flags    | ication-key-file |   |   | {. |      |
|      |      |              | OR               |   |   | un |      |
|      |      | \--verificat |                  |   |   | de |      |
|      |      | ion-key-file | \--              |   |   | rl |      |
|      |      |              | signing-key-file |   |   | in |      |
|      |      | \--sign      | parameters       |   |   | e} |      |
|      |      | ing-key-file | **THEN** the     |   |   | ]( |      |
|      |      |              | command fails    |   |   | ht |      |
|      |      | fails with   | and returns an   |   |   | tp |      |
|      |      | an           | error to the     |   |   | s: |      |
|      |      | appropriate  | users informing  |   |   | // |      |
|      |      | error        | them to fill     |   |   | gi |      |
|      |      | message.     | those parameters |   |   | th |      |
|      |      |              | in. The error    |   |   | ub |      |
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
|      |      | **re         | **resign_com     |   |   |    |      |
|      |      | sign_committ | mittee_cold_cert |   |   |    |      |
|      |      | ee_cold_cert | = (15,           |   |   |    |      |
|      |      | = (15,       | committee_       |   |   |    |      |
|      |      | co           | cold_credential, |   |   |    |      |
|      |      | mmittee_cold | anchor / null)** |   |   |    |      |
|      |      | _credential, |                  |   |   |    |      |
|      |      | anchor /     |                  |   |   |    |      |
|      |      | null)**      |                  |   |   |    |      |
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
|      |      |              | **not**          |   |   |    |      |
|      |      |              | specified, the   |   |   |    |      |
|      |      |              | DRep ID should   |   |   |    |      |
|      |      |              | be displayed in  |   |   |    |      |
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
|      |      | [The feature | **Detail         |   |   |    |      |
|      |      | im           | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | should       | Pending**        |   |   |    |      |
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
|      | tire | [**Using**   | certificate.     |   |   |    |      |
|      | ment | the          |                  |   |   |    |      |
|      | (unr | \--drep-veri |                  |   |   |    |      |
|      | egis | fication-key |                  |   |   |    |      |
|      | trat | STRING       |                  |   |   |    |      |
|      | ion) | option to    |                  |   |   |    |      |
|      | cer  | specify the  |                  |   |   |    |      |
|      | tifi | DRep         |                  |   |   |    |      |
|      | cate | verification |                  |   |   |    |      |
|      |      | key directly |                  |   |   |    |      |
|      | So   | as a         |                  |   |   |    |      |
|      | that | str          |                  |   |   |    |      |
|      | I    | ing.]{.mark} |                  |   |   |    |      |
|      | can  |              |                  |   |   |    |      |
|      | su   | [**Using**   |                  |   |   |    |      |
|      | bmit | the          |                  |   |   |    |      |
|      | it   | \--dr        |                  |   |   |    |      |
|      | on a | ep-verificat |                  |   |   |    |      |
|      | tra  | ion-key-file |                  |   |   |    |      |
|      | nsac | FILE option  |                  |   |   |    |      |
|      | tion | to specify   |                  |   |   |    |      |
|      | and  | the file     |                  |   |   |    |      |
|      | can  | containing   |                  |   |   |    |      |
|      | get  | the DRep     |                  |   |   |    |      |
|      | my   | verification |                  |   |   |    |      |
|      | DRep | key.]{.mark} |                  |   |   |    |      |
|      | dep  |              |                  |   |   |    |      |
|      | osit | [**Using**   |                  |   |   |    |      |
|      | b    | the          |                  |   |   |    |      |
|      | ack. | \--drep-id   |                  |   |   |    |      |
|      |      | STRING       |                  |   |   |    |      |
|      |      | option to    |                  |   |   |    |      |
|      |      | specify the  |                  |   |   |    |      |
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
|      |      | [The output  | **Detail         |   |   |    |      |
|      |      | certificate  | Pending**        |   |   |    |      |
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
|      |      | [The feature | **Detail         |   |   |    |      |
|      |      | im           | Pending**        |   |   |    |      |
|      |      | plementation |                  |   |   |    |      |
|      |      | should be    |                  |   |   |    |      |
|      |      | well         |                  |   |   |    |      |
|      |      | -documented, |                  |   |   |    |      |
|      |      | providing    |                  |   |   |    |      |
|      |      | clear usage  |                  |   |   |    |      |
|      |      | instruct     |                  |   |   |    |      |
|      |      | ions]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | handles      | Pending**        |   |   |    |      |
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
| C    | As a | [The command | **Detail         |   |   |    |      |
| LI12 | Drep | calculates   | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | supports the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | handles      | Pending**        |   |   |    |      |
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
| C    | As   | [The command | **Detail         |   |   |    |      |
| LI13 | an   | requires     | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | allows the   | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the      | Pending**        |   |   |    |      |
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
|      |      | [The         | **Detail         |   |   |    |      |
|      |      | generated    | Pending**        |   |   |    |      |
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
| C    | As   | [The command | **Detail         |   |   |    |      |
| LI14 | an   | requires     | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | offers the   | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | offers the   | Pending**        |   |   |    |      |
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
|      |      | [When adding | **Detail         |   |   |    |      |
|      |      | a new        | Pending**        |   |   |    |      |
|      |      | member, the  |                  |   |   |    |      |
|      |      | command      |                  |   |   |    |      |
|      |      | requires the |                  |   |   |    |      |
|      |      | user to also |                  |   |   |    |      |
|      |      | provide a    |                  |   |   |    |      |
|      |      | **term** for |                  |   |   |    |      |
|      |      | each new     |                  |   |   |    |      |
|      |      | member using |                  |   |   |    |      |
|      |      | the flag     |                  |   |   |    |      |
|      |      | **--epo      |                  |   |   |    |      |
|      |      | ch**]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | allows       | Pending**        |   |   |    |      |
|      |      | proposing a  |                  |   |   |    |      |
|      |      | new quorum   |                  |   |   |    |      |
|      |      | thresh       |                  |   |   |    |      |
|      |      | old:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [**When**  |                  |   |   |    |      |
|      |      | > adding     |                  |   |   |    |      |
|      |      | > mem        |                  |   |   |    |      |
|      |      | bers]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [**When**  |                  |   |   |    |      |
|      |      | > removing   |                  |   |   |    |      |
|      |      | > mem        |                  |   |   |    |      |
|      |      | bers]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [**As**    |                  |   |   |    |      |
|      |      | > standalone |                  |   |   |    |      |
|      |      | > action (no |                  |   |   |    |      |
|      |      | > adds or    |                  |   |   |    |      |
|      |      | > remov      |                  |   |   |    |      |
|      |      | als)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
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
|      |      | [The         | **Detail         |   |   |    |      |
|      |      | generated    | Pending**        |   |   |    |      |
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
| C    | As   | [The command | **Detail         |   |   |    |      |
| LI15 | an   | requires     | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [Requires    | **Detail         |   |   |    |      |
|      |      | the user to  | Pending**        |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | **amount**   |                  |   |   |    |      |
|      |      | in lovelace  |                  |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
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
|      |      | [The         | **Detail         |   |   |    |      |
|      |      | generated    | Pending**        |   |   |    |      |
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
| C    | As   | [The command | **Detail         |   |   |    |      |
| LI16 | an   | requires     | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
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
|      |      | [The         | **Detail         |   |   |    |      |
|      |      | generated    | Pending**        |   |   |    |      |
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
| C    | As   | [The command | **Detail         |   |   |    |      |
| LI17 | an   | requires     | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | allows the   | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | includes     | Pending**        |   |   |    |      |
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
|      |      | [The         |                  |   |   |    |      |
|      |      | **network    |                  |   |   |    |      |
|      |      | group**      |                  |   |   |    |      |
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
|      |      | **economic   |                  |   |   |    |      |
|      |      | group**      |                  |   |   |    |      |
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
|      |      | **technical  |                  |   |   |    |      |
|      |      | group**      |                  |   |   |    |      |
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
|      |      | **governance |                  |   |   |    |      |
|      |      | group**      |                  |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
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
|      |      | [The         | **Detail         |   |   |    |      |
|      |      | generated    | Pending**        |   |   |    |      |
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
| C    | As   | [The command | **Detail         |   |   |    |      |
| LI18 | an   | requires     | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | allows the   | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
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
|      |      | [The         | **Detail         |   |   |    |      |
|      |      | generated    | Pending**        |   |   |    |      |
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
| C    | As   | [The command | **Detail         |   |   |    |      |
| LI19 | an   | requires     | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | allows the   | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | input the    |                  |   |   |    |      |
|      |      | **new        |                  |   |   |    |      |
|      |      | protocol     |                  |   |   |    |      |
|      |      | version      |                  |   |   |    |      |
|      |      | numb         |                  |   |   |    |      |
|      |      | er**]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
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
|      |      | [The         | **Detail         |   |   |    |      |
|      |      | generated    | Pending**        |   |   |    |      |
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
| C    | As   | [The command | **Detail         |   |   |    |      |
| LI20 | an   | takes an     | Pending**        |   |   |    |      |
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
|      |      | [Gives an    | **Detail         |   |   |    |      |
|      |      | option to    | Pending**        |   |   |    |      |
|      |      | select the   |                  |   |   |    |      |
|      |      | output       |                  |   |   |    |      |
|      |      | format (json |                  |   |   |    |      |
|      |      | or           |                  |   |   |    |      |
|      |      | y            |                  |   |   |    |      |
|      |      | aml)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
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
|      |      | [The output  | **Detail         |   |   |    |      |
|      |      | shows the    | Pending**        |   |   |    |      |
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
| C    | As a | [The command | **Detail         |   |   |    |      |
| LI21 | D    | provides a   | Pending**        |   |   |    |      |
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
|      |      | [Requires to | **Detail         |   |   |    |      |
|      |      | specify the  | Pending**        |   |   |    |      |
|      |      | governance   |                  |   |   |    |      |
|      |      | action ID    |                  |   |   |    |      |
|      |      | and index    |                  |   |   |    |      |
|      |      | that the     |                  |   |   |    |      |
|      |      | vote is      |                  |   |   |    |      |
|      |      | ab           |                  |   |   |    |      |
|      |      | out.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Requires    | **Detail         |   |   |    |      |
|      |      | the user to  | Pending**        |   |   |    |      |
|      |      | provide      |                  |   |   |    |      |
|      |      | DRep, SPO or |                  |   |   |    |      |
|      |      | CC           |                  |   |   |    |      |
|      |      | credent      |                  |   |   |    |      |
|      |      | ials]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | allows the   | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | vote will be |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The         | **Detail         |   |   |    |      |
|      |      | generated    | Pending**        |   |   |    |      |
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
| C    | As a | [The command | **Detail         |   |   |    |      |
| LI22 | D    | takes a vote | Pending**        |   |   |    |      |
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
|      |      | [Gives an    | **Detail         |   |   |    |      |
|      |      | option to    | Pending**        |   |   |    |      |
|      |      | select the   |                  |   |   |    |      |
|      |      | output       |                  |   |   |    |      |
|      |      | format (json |                  |   |   |    |      |
|      |      | or           |                  |   |   |    |      |
|      |      | y            |                  |   |   |    |      |
|      |      | aml)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
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
|      |      | [The output  | **Detail         |   |   |    |      |
|      |      | shows the    | Pending**        |   |   |    |      |
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
| C    | As   | [Transaction | **Detail         |   |   |    |      |
| LI23 | an   | **build**    | Pending**        |   |   |    |      |
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
+------+------+--------------+------------------+---+---+----+------+
|      |      | [When        | **Detail         |   |   |    |      |
|      |      | constructing | Pending**        |   |   |    |      |
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
|      |      | **[, ? 20 :  |                  |   |   |    |      |
|      |      | proposa      |                  |   |   |    |      |
|      |      | l_procedures |                  |   |   |    |      |
|      |      | ; New;       |                  |   |   |    |      |
|      |      | Proposal     |                  |   |   |    |      |
|      |      | procedur     |                  |   |   |    |      |
|      |      | es]{.mark}** |                  |   |   |    |      |
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
| C    | As a | [Transaction | **Detail         |   |   |    |      |
| LI24 | D    | **build**    | Pending**        |   |   |    |      |
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
+------+------+--------------+------------------+---+---+----+------+
|      |      | [When        | **Detail         |   |   |    |      |
|      |      | constructing | Pending**        |   |   |    |      |
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
|      |      | **[, ? 19 :  |                  |   |   |    |      |
|      |      | votin        |                  |   |   |    |      |
|      |      | g_procedures |                  |   |   |    |      |
|      |      | ; New;       |                  |   |   |    |      |
|      |      | Voting       |                  |   |   |    |      |
|      |      | procedur     |                  |   |   |    |      |
|      |      | es]{.mark}** |                  |   |   |    |      |
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
| C    | As   | [Transaction | **Detail         |   |   |    |      |
| LI25 | an   | build-raw    | Pending**        |   |   |    |      |
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
|      |      | [When        | **Detail         |   |   |    |      |
|      |      | constructing | Pending**        |   |   |    |      |
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
|      |      | **[, ? 20 :  |                  |   |   |    |      |
|      |      | proposa      |                  |   |   |    |      |
|      |      | l_procedures |                  |   |   |    |      |
|      |      | ; New;       |                  |   |   |    |      |
|      |      | Proposal     |                  |   |   |    |      |
|      |      | procedur     |                  |   |   |    |      |
|      |      | es]{.mark}** |                  |   |   |    |      |
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
| C    | As a | [Transaction | **Detail         |   |   |    |      |
| LI26 | D    | build-raw    | Pending**        |   |   |    |      |
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
|      |      | [When        | **Detail         |   |   |    |      |
|      |      | constructing | Pending**        |   |   |    |      |
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
|      |      | **[, ? 19 :  |                  |   |   |    |      |
|      |      | votin        |                  |   |   |    |      |
|      |      | g_procedures |                  |   |   |    |      |
|      |      | ; New;       |                  |   |   |    |      |
|      |      | Voting       |                  |   |   |    |      |
|      |      | procedur     |                  |   |   |    |      |
|      |      | es]{.mark}** |                  |   |   |    |      |
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
| C    | As   | [Allows the  | **Detail         |   |   |    |      |
| LI27 | an   | user to      | Pending**        |   |   |    |      |
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
|      |      | [Requires    | **Detail         |   |   |    |      |
|      |      | the user to  | Pending**        |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | required key |                  |   |   |    |      |
|      |      | deposit in   |                  |   |   |    |      |
|      |      | love         |                  |   |   |    |      |
|      |      | lace]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | handles      | Pending**        |   |   |    |      |
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
|      |      | [The         | **Detail         |   |   |    |      |
|      |      | certificate  | Pending**        |   |   |    |      |
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
|      |      | [The         | **Detail         |   |   |    |      |
|      |      | resulting    | Pending**        |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | conforms     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl, |                  |   |   |    |      |
|      |      | where\       |                  |   |   |    |      |
|      |      | \            |                  |   |   |    |      |
|      |      | **reg_cert = |                  |   |   |    |      |
|      |      | (7,          |                  |   |   |    |      |
|      |      | stake        |                  |   |   |    |      |
|      |      | _credential, |                  |   |   |    |      |
|      |      | coi          |                  |   |   |    |      |
|      |      | n)**]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [Allows the  | **Detail         |   |   |    |      |
| LI28 | an   | user to      | Pending**        |   |   |    |      |
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
|      |      | [Requires    | **Detail         |   |   |    |      |
|      |      | the user to  | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | handles      | Pending**        |   |   |    |      |
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
|      |      | [The         | **Detail         |   |   |    |      |
|      |      | certificate  | Pending**        |   |   |    |      |
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
|      |      | [The         | **Detail         |   |   |    |      |
|      |      | resulting    | Pending**        |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | conforms     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl, |                  |   |   |    |      |
|      |      | where\       |                  |   |   |    |      |
|      |      | \            |                  |   |   |    |      |
|      |      | **unreg_cert |                  |   |   |    |      |
|      |      | = (8,        |                  |   |   |    |      |
|      |      | stake        |                  |   |   |    |      |
|      |      | _credential, |                  |   |   |    |      |
|      |      | coi          |                  |   |   |    |      |
|      |      | n)**]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [Allows the  | **Detail         |   |   |    |      |
| LI29 | an   | user to      | Pending**        |   |   |    |      |
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
|      |      | [When        | **Detail         |   |   |    |      |
|      |      | delegating   | Pending**        |   |   |    |      |
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
|      |      | [When        | **Detail         |   |   |    |      |
|      |      | delegating   | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | handles      | Pending**        |   |   |    |      |
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
|      |      | [The         | **Detail         |   |   |    |      |
|      |      | certificate  | Pending**        |   |   |    |      |
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
|      |      | [The         | **Detail         |   |   |    |      |
|      |      | resulting    | Pending**        |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | conforms     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl, |                  |   |   |    |      |
|      |      | where\       |                  |   |   |    |      |
|      |      | \            |                  |   |   |    |      |
|      |      | **vot        |                  |   |   |    |      |
|      |      | e_deleg_cert |                  |   |   |    |      |
|      |      | = (9,        |                  |   |   |    |      |
|      |      | stake        |                  |   |   |    |      |
|      |      | _credential, |                  |   |   |    |      |
|      |      | dre          |                  |   |   |    |      |
|      |      | p)**]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [Allows the  | **Detail         |   |   |    |      |
| LI30 | an   | user to      | Pending**        |   |   |    |      |
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
|      |      | [The user    | **Detail         |   |   |    |      |
|      |      | can provide  | Pending**        |   |   |    |      |
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
|      |      | [Allows the  | **Detail         |   |   |    |      |
|      |      | user to      | Pending**        |   |   |    |      |
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
|      |      | [When        | **Detail         |   |   |    |      |
|      |      | delegating   | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | handles      | Pending**        |   |   |    |      |
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
|      |      | [The         | **Detail         |   |   |    |      |
|      |      | certificate  | Pending**        |   |   |    |      |
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
|      |      | [The         | **Detail         |   |   |    |      |
|      |      | resulting    | Pending**        |   |   |    |      |
|      |      | certificate  |                  |   |   |    |      |
|      |      | conforms     |                  |   |   |    |      |
|      |      | with the     |                  |   |   |    |      |
|      |      | conway cddl, |                  |   |   |    |      |
|      |      | where\       |                  |   |   |    |      |
|      |      | \            |                  |   |   |    |      |
|      |      | **stake_vot  |                  |   |   |    |      |
|      |      | e_deleg_cert |                  |   |   |    |      |
|      |      | = (10,       |                  |   |   |    |      |
|      |      | stake        |                  |   |   |    |      |
|      |      | _credential, |                  |   |   |    |      |
|      |      | p            |                  |   |   |    |      |
|      |      | ool_keyhash, |                  |   |   |    |      |
|      |      | dre          |                  |   |   |    |      |
|      |      | p)**]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| C    | As   | [The new     | **Detail         |   |   |    |      |
| LI31 | any  | command is   | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | requires the | Pending**        |   |   |    |      |
|      |      | user to      |                  |   |   |    |      |
|      |      | specify the  |                  |   |   |    |      |
|      |      | network id   |                  |   |   |    |      |
|      |      | (mainnet or  |                  |   |   |    |      |
|      |      | testnet      |                  |   |   |    |      |
|      |      | ma           |                  |   |   |    |      |
|      |      | gic)]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | output will  |                  |   |   |    |      |
|      |      | be           |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The output  | **Detail         |   |   |    |      |
|      |      | is a JSON    | Pending**        |   |   |    |      |
|      |      | showing, at  |                  |   |   |    |      |
|      |      | least, the   |                  |   |   |    |      |
|      |      | following    |                  |   |   |    |      |
|      |      | informat     |                  |   |   |    |      |
|      |      | ion:]{.mark} |                  |   |   |    |      |
|      |      |              |                  |   |   |    |      |
|      |      | > [          |                  |   |   |    |      |
|      |      | **Previous** |                  |   |   |    |      |
|      |      | > protocol   |                  |   |   |    |      |
|      |      | > parame     |                  |   |   |    |      |
|      |      | ters]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | [**Current** |                  |   |   |    |      |
|      |      | > protocol   |                  |   |   |    |      |
|      |      | > parame     |                  |   |   |    |      |
|      |      | ters]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | > [**Last**  |                  |   |   |    |      |
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
|      |      | > [          |                  |   |   |    |      |
|      |      | **Ratified** |                  |   |   |    |      |
|      |      | > governance |                  |   |   |    |      |
|      |      | > actions    |                  |   |   |    |      |
|      |      | > that will  |                  |   |   |    |      |
|      |      | > be enacted |                  |   |   |    |      |
|      |      | > at next    |                  |   |   |    |      |
|      |      | > epoch      |                  |   |   |    |      |
|      |      | > transi     |                  |   |   |    |      |
|      |      | tion]{.mark} |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      | >            |                  |   |   |    |      |
|      |      |  [**Active** |                  |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | handles      | Pending**        |   |   |    |      |
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
| C    | As a | [The command | **Detail         |   |   |    |      |
| LI32 | CC   | is           | Pending**        |   |   |    |      |
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
|      |      | [Requires    | **Detail         |   |   |    |      |
|      |      | the user to  | Pending**        |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | network      |                  |   |   |    |      |
|      |      | id]{.mark}   |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Supports a  | **Detail         |   |   |    |      |
|      |      | query for an | Pending**        |   |   |    |      |
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
|      |      | [When no CC  | **Detail         |   |   |    |      |
|      |      | key is       | Pending**        |   |   |    |      |
|      |      | specified,   |                  |   |   |    |      |
|      |      | the command  |                  |   |   |    |      |
|      |      | outputs      |                  |   |   |    |      |
|      |      | information  |                  |   |   |    |      |
|      |      | for all      |                  |   |   |    |      |
|      |      | committee    |                  |   |   |    |      |
|      |      | mem          |                  |   |   |    |      |
|      |      | bers]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | allows       | Pending**        |   |   |    |      |
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
|      |      | [The output  | **Detail         |   |   |    |      |
|      |      | is a JSON    | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | output will  |                  |   |   |    |      |
|      |      | be           |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | handles      | Pending**        |   |   |    |      |
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
| C    | As   | [The command | **Detail         |   |   |    |      |
| LI33 | an   | is           | Pending**        |   |   |    |      |
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
|      |      | [Requires    | **Detail         |   |   |    |      |
|      |      | the user to  | Pending**        |   |   |    |      |
|      |      | provide the  |                  |   |   |    |      |
|      |      | network      |                  |   |   |    |      |
|      |      | id]{.mark}   |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [Supports a  | **Detail         |   |   |    |      |
|      |      | query for an | Pending**        |   |   |    |      |
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
|      |      | [If no Drep  | **Detail         |   |   |    |      |
|      |      | credential   | Pending**        |   |   |    |      |
|      |      | is specified |                  |   |   |    |      |
|      |      | it returns   |                  |   |   |    |      |
|      |      | all          |                  |   |   |    |      |
|      |      | D            |                  |   |   |    |      |
|      |      | Reps]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | output will  |                  |   |   |    |      |
|      |      | be           |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The output  | **Detail         |   |   |    |      |
|      |      | is a JSON    | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | handles      | Pending**        |   |   |    |      |
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
| C    | As   | [The command | **Detail         |   |   |    |      |
| LI34 | an   | is           | Pending**        |   |   |    |      |
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
|      |      | [Supports a  | **Detail         |   |   |    |      |
|      |      | query for an | Pending**        |   |   |    |      |
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
|      |      | [If no Drep  | **Detail         |   |   |    |      |
|      |      | credential   | Pending**        |   |   |    |      |
|      |      | is specified |                  |   |   |    |      |
|      |      | it returns   |                  |   |   |    |      |
|      |      | all          |                  |   |   |    |      |
|      |      | D            |                  |   |   |    |      |
|      |      | Reps]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | has the flag | Pending**        |   |   |    |      |
|      |      | --out-file   |                  |   |   |    |      |
|      |      | to specify   |                  |   |   |    |      |
|      |      | the file     |                  |   |   |    |      |
|      |      | where the    |                  |   |   |    |      |
|      |      | output will  |                  |   |   |    |      |
|      |      | be           |                  |   |   |    |      |
|      |      | sa           |                  |   |   |    |      |
|      |      | ved.]{.mark} |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      |      | [The output  | **Detail         |   |   |    |      |
|      |      | is a JSON    | Pending**        |   |   |    |      |
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
|      |      | [The command | **Detail         |   |   |    |      |
|      |      | handles      | Pending**        |   |   |    |      |
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
| CH.  | As a | [[Jon        | **Detail         |   | * | S  |      |
| SID1 | Si   | Rossie       | Pending**        |   | * | id |      |
|      | dech | ]{.underline |                  |   | D | ec |      |
|      | ain, | }](mailto:jo |                  |   | e | ha |      |
|      | I    | n.rossie@ioh |                  |   | t | in |      |
|      | wish | k.io)[posted |                  |   | a |    |      |
|      | to   | your 'thread |                  |   | i |    |      |
|      | use  | comments' to |                  |   | l |    |      |
|      | BLS  | init         |                  |   | P |    |      |
|      | pr   | iate]{.mark} |                  |   | e |    |      |
|      | imit |              |                  |   | n |    |      |
|      | ives |              |                  |   | d |    |      |
|      | to   |              |                  |   | i |    |      |
|      | re   |              |                  |   | n |    |      |
|      | cord |              |                  |   | g |    |      |
|      | se   |              |                  |   | * |    |      |
|      | ttle |              |                  |   | * |    |      |
|      | ment |              |                  |   |   |    |      |
|      | op   |              |                  |   |   |    |      |
|      | erat |              |                  |   |   |    |      |
|      | ions |              |                  |   |   |    |      |
|      | on   |              |                  |   |   |    |      |
|      | Car  |              |                  |   |   |    |      |
|      | dano |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
| CH.  | S    | Detail       | **Detail         |   | * | S  |      |
| SID2 | idec | Pending      | Pending**        |   | * | id |      |
|      | hain |              |                  |   | D | ec |      |
|      | will |              |                  |   | e | ha |      |
|      | use  |              |                  |   | t | in |      |
|      | BLS  |              |                  |   | a |    |      |
|      | for  |              |                  |   | i |    |      |
|      | tok  |              |                  |   | l |    |      |
|      | enom |              |                  |   | P |    |      |
|      | ics, |              |                  |   | e |    |      |
|      | in   |              |                  |   | n |    |      |
|      | pa   |              |                  |   | d |    |      |
|      | rtic |              |                  |   | i |    |      |
|      | ular |              |                  |   | n |    |      |
|      | to   |              |                  |   | g |    |      |
|      | sup  |              |                  |   | * |    |      |
|      | port |              |                  |   | * |    |      |
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
| CI   | As a | Sums         | **Detail         |   |   | Pl |      |
| P-85 | DApp | -of-products | Pending**        |   |   | ut |      |
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
| CIP  | User | Detail       | **Detail         |   |   | Pl |      |
| -101 | sto  | Pending      | Pending**        |   |   | ut |      |
|      | ries |              |                  |   |   | us |      |
|      | for  |              |                  |   |   |    |      |
|      | K    |              |                  |   |   |    |      |
|      | ecca |              |                  |   |   |    |      |
|      | k256 |              |                  |   |   |    |      |
|      | p    |              |                  |   |   |    |      |
|      | rimi |              |                  |   |   |    |      |
|      | tive |              |                  |   |   |    |      |
+------+------+--------------+------------------+---+---+----+------+
|      | As a | The          | **Detail         |   |   | Pl |      |
|      | DApp | Blake2b-224  | Pending**        |   |   | ut |      |
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
