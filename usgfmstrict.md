# Document Summary

Upon socialising of this Inventory, and eventual agreement, we will
progress to detailing how the Acceptance will be accomplished and
signoff achieved, the ‘Accepted’ column will be marked Yes once
consensus is reached.

# Change Management

Upon agreement on the User Story Inventory, a suitable level of Change
Management will be applied, this will enable us to phase-deliver
Governance on Cardano and to fulfil the ongoing Ecosystem and Community
needs. Additional User Stories will be proposed, reviewed, approved and
accepted using

# Source Areas Under Consideration

This section shows the areas or sources thus far

<table style="width:49%;">
<colgroup>
<col style="width: 7%" />
<col style="width: 15%" />
<col style="width: 12%" />
<col style="width: 12%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Source</strong></th>
<th><strong>Outline Contribution</strong></th>
<th><strong>State</strong></th>
<th><strong>Key Contract</strong></th>
</tr>
<tr class="odd">
<th>Voltaire</th>
<th>Use Cases for Governance, voting, delegation</th>
<th>Initial Capture Complete</th>
<th>Outreach in progress</th>
</tr>
<tr class="header">
<th>CIP-1694</th>
<th>Blockchain level User Stories on voting, delegation, identity,
consensus</th>
<th>Initial Capture Complete</th>
<th>Outreach in progress</th>
</tr>
<tr class="odd">
<th>Smart Contracts</th>
<th>Plutus v3 and BLS</th>
<th>Initial Capture Complete</th>
<th>Outreach in progress</th>
</tr>
<tr class="header">
<th>CLI-API</th>
<th>Interface outline and definition</th>
<th>Initial Capture Complete</th>
<th>Outreach in progress</th>
</tr>
<tr class="odd">
<th>Sidechains</th>
<th>Interaction with BLS primitives</th>
<th>Outreach in progress</th>
<th>Outreach in progress</th>
</tr>
<tr class="header">
<th>DApps</th>
<th>To be defined and elaborated</th>
<th>To be defined</th>
<th>Outreach in progress</th>
</tr>
<tr class="odd">
<th>Exchanges</th>
<th>To be defined and elaborated</th>
<th>To be defined</th>
<th>Outreach in progress</th>
</tr>
<tr class="header">
<th>Other</th>
<th>To be defined and elaborated</th>
<th>To be defined</th>
<th>Outreach in progress</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

# User Story (Voltaire, API, CIP-1694, Community et al)

<table>
<colgroup>
<col style="width: 10%" />
<col style="width: 10%" />
<col style="width: 21%" />
<col style="width: 27%" />
<col style="width: 4%" />
<col style="width: 6%" />
<col style="width: 8%" />
<col style="width: 10%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>UID</strong></th>
<th><strong>User Story</strong></th>
<th><strong>Functional Requirement</strong></th>
<th><strong>Acceptance Criteria</strong></th>
<th><strong>Link</strong></th>
<th><strong>Accepted</strong></th>
<th><strong>Source</strong></th>
<th><strong>Enabler(Y,N)</strong></th>
</tr>
<tr class="odd">
<th rowspan="11">CH.VO1</th>
<th rowspan="11">As a DRep or Ada Holder <strong>I want to connect my
wallet to GovTool</strong> so that I can post transactions on-chain</th>
<th rowspan="4">Connect with multiple stake key wallet</th>
<th><p>Given I am on the homepage</p>
<p>And my wallet is not connected.</p>
<p>When I click the Connect Wallet button</p>
<p>And select (one of) my CIP-95 compatible wallet(s) with multiple
stake keys</p>
<p>And select from a list which stake key I wish to connect with</p>
<p>Then the wallet will prompt me to connect and I can connect to
GovTool with it on the selected stake key.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th><p>Given I am on the homepage</p>
<p>And my wallet is not connected</p>
<p>When I click the Connect Wallet button</p>
<p>Then I am not shown any non CIP-95 compatible wallets.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th><p>Given I am on the homepage</p>
<p>And my wallet is not connected</p>
<p>When I click the Connect Wallet button and select a CIP-95 compliant,
multiple stake key wallet, containing zero ADA (or tADA for
SanchoNet)</p>
<p>Then a modal window opens showing my CIP-95 compatible wallets</p>
<p>When I select a wallet with multiple stake keys from this list</p>
<p>Then I am asked which stake key I wish to connect with</p>
<p>When I select a stake key</p>
<p>Then the wallet opens and I can connect with it on the selected stake
key.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th><p>Given i am on the homepage without my wallet connected</p>
<p>When I click the Connect Wallet button and select a CIP-95 compliant,
single stake key wallet, containing more than zero ADA (or tADA for
SanchoNet)</p>
<p>Then a modal window opens showing my CIP-95 compatible wallets</p>
<p>When I select a wallet with multiple stake keys from this list</p>
<p>Then I am asked which stake key I wish to connect with</p>
<p>When I select a stake key</p>
<p>Then the wallet opens and I can connect with it on the selected stake
key.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th rowspan="4">Connect with single stake key wallet</th>
<th><p>Given I am on the homepage with no wallet connected</p>
<p>When I click the Connect Wallet button and select a CIP-95 compliant
single stake key wallet</p>
<p>Then my wallet appears and I can connect with it</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th><p>Given I am on the homepage without my wallet connected</p>
<p>When I click the Connect Wallet button</p>
<p>Then I am not shown any non CIP-95 compatible wallets.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th><p>Given I am on the homepage without my wallet connected</p>
<p>When I click the Connect Wallet button and select a CIP-95 compliant,
single stake key wallet, containing zero ADA (or tADA for SanchoNet)</p>
<p>Then my wallet appears and I can connect with it</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th><p>Given I am on the homepage without my wallet connected</p>
<p>When I click the Connect Wallet button and select a CIP-95 compliant,
single stake key wallet, containing more than zero ADA (or tADA for
SanchoNet)</p>
<p>Then my wallet appears and I can connect with it</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th rowspan="2">Disconnect wallet</th>
<th><p>Given that I am on the dashboard with my wallet connected</p>
<p>If I click the Disconnect button</p>
<p>Then my wallet is disconnected from GovTool and I am redirected to
the homepage.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th><p>Given that I am connected to GovTool with my wallet</p>
<p>When I disconnect</p>
<p>Then I will be redirected to the homepage, and will not have access
to delegation or voting features.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th>Check the wallet is on the correct network</th>
<th><p>Given I am on the homepage<br />
<br />
When I compare the networkId with the environment value set on the
deployment for the network.</p>
<p>Then if there are exceptions raised, fail the test.</p>
<p>If no exceptions, connect the wallet to the network (pass)</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th rowspan="17">CH.VO2</th>
<th rowspan="17">As an Ada Holder <strong>I want to</strong>
<strong>delegate my voting power</strong> to a DRep so that I can claim
my staking rewards</th>
<th rowspan="3">Delegate to DRep ID</th>
<th><p>Given that I have my wallet connected, and I am on the Delegate
to DRep page</p>
<p>When I select the delegate to DRep ID option and I enter a DRep ID
which has not been registered and I press delegate</p>
<p>Then I will be presented with an error message explaining that the
DRep ID was not found.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th><p>Given that I have my wallet connected, and I am on the delegate
to DRep page,</p>
<p>When I choose the Delegate to DRep ID option and I enter a registered
DRep ID and I press the Delegate button</p>
<p>Then I am able to delegate to that DRep ID via my connected
wallet</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th><p>Given that I have connected to GovTool with zero* ADA (or tADA in
the case of SanchoNet)</p>
<p>When I choose the Delegate to DRep ID option and I enter a registered
DRep ID and I press the Delegate button</p>
<p>Then I am presented with a warning message and cannot proceed with
delegation.</p>
<p>*or at least a number below transaction costs</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th rowspan="2">Access Delegate to DRep page</th>
<th><p>Given that I do not have a compatible wallet connected to
GovTool</p>
<p>When I attempt to visit the URL of the Delegate to DRep page</p>
<p>Then I am redirected to the homepage</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th><p>Given that I have a compatible wallet connected to GovTool and I
am looking at the dashboard</p>
<p>When I click on the the Delegate button (or Change Delegation button
if you are already registered)</p>
<p>Then I am shown the Delegate to DRep page</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th>Verify DRep behaviour in connected state</th>
<th><p>Given that I'm not connected to the wallet</p>
<p>When I visit the DRep delegation page, and I click the
delegate-connect-wallet-button</p>
<p>Then the connect your wallet-modal is visible</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th>Verify DRep behaviour in disconnected state</th>
<th><p>Given that I have a preset DRep wallet loaded</p>
<p>Then Delegate button is clicked</p>
<p>Then it is expected that delegation options card is visible</p>
<p>delegate to myself is expected to be visible</p>
<p>Then Other options is clicked</p>
<p>Expect that signal no confidence card and vote abstain cards are
visible</p>
<p>Next, delegate to dRep card is clicked, followed by next step
button</p>
<p>Then expected that dRep ID input is visible along with delegate
button</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th rowspan="3">Delegate to myself</th>
<th><p>Given that I am a registered DRep who is connected to GovTool
with my wallet, and I am on the Delegate to DRep page</p>
<p>When I choose the Delegate to DRep ID option and I enter my own DRep
ID and I press the Delegate button</p>
<p>Then I am able to delegate to myself via my connected wallet</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th><p>Given that I am a registered DRep who is connected to GovTool
with my wallet, and I am on the Delegate to DRep page</p>
<p>When I select the Delegate to Myself option and press the Delegate
button</p>
<p>Then I will be able to send a transaction to delegate to myself via
my wallet</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th><p>Given that I am not a registered DRep, and I am connected to
GovTool with my wallet,</p>
<p>When I am on the Delegate to DRep page</p>
<p>I cannot see a Delegate to Myself option</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th rowspan="2">Change my DRep delegation</th>
<th><p>Given that I am I am already delegated to a DRep</p>
<p>When I look at the dashboard</p>
<p>GovTool will know that I am delegated and it will invite me to
“change my delegation” rather than to delegate.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th><p>Given that I am already delegated</p>
<p>When I go to change my delegation</p>
<p>I can delegate to any registered DRep, If I am delegated to myself
then the option to “delegate to myself” will not be shown, If I am
delegated to a specific predefined DRep then this predefined option will
not be shown.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th>Check the validity of a DRep ID</th>
<th>Given that I have selected the “delegate to a DRep ID” option in the
delegation user journey.<br />
<br />
When I enter anything in the DRep ID input box that is not a registered
DRep ID.<br />
<br />
Then I will not be able to delegate to this DRep ID and will get a
warning message.</th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th rowspan="2">Delegate to Abstain</th>
<th><p>Given that I am a DRep</p>
<p>When I delegate using the “delegate to abstain” feature</p>
<p>Then it will only delegate my own lovelace’s voting power to Abstain
and NOT the voting power (if any) that has been delegated to me by
others. I will be notified that my delegation transaction was
sent.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th></th>
</tr>
<tr class="header">
<th><p>Given that I am not a DRep</p>
<p>When I delegate using the “delegate to abstain” feature</p>
<p>Then it will delegate any voting power I have to Abstain. I will be
notified that my delegation transaction was sent.</p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="2">Delegate to No-Confidence</th>
<th><p>Given that I am a DRep</p>
<p>When I delegate using the “delegate to no-confidence” feature</p>
<p>Then it will only delegate my own lovelace’s voting power to
No-Confidence and NOT the voting power (if any) that has been delegated
to me by others. I will be notified that my delegation transaction was
sent.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th></th>
</tr>
<tr class="header">
<th><p>Given that I am not a DRep</p>
<p>When I delegate using the “delegate to no-confidence” feature</p>
<p>Then it will delegate any voting power I have to No-Confi. I will be
notified that my delegation transaction was sent.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th></th>
</tr>
<tr class="odd">
<th></th>
<th></th>
<th>Guardrails for Voltaire</th>
<th>This work is in progress</th>
<th></th>
<th></th>
<th>Voltaire</th>
<th></th>
</tr>
<tr class="header">
<th rowspan="5">CH.VO3</th>
<th rowspan="5"><strong>As a DRep I want to register</strong> so that I
can vote on governance actions</th>
<th rowspan="3">Register as a DRep</th>
<th><p>Given that I am connected to GovTool with a compatible wallet</p>
<p>When I go through the DRep registration process, and do not include a
metadata anchor</p>
<p>Then I can register as a DRep via my wallet (because metadata anchors
are optional)</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th><p>Given that I am connected to GovTool with a compatible wallet</p>
<p>When I go through the DRep registration process, and include metadata
anchor information in the wrong format</p>
<p>Then I will not be able to progress further in the process and I will
be told that it is because the format is incorrect.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th><p>Given that I am connected to GovTool with a compatible wallet</p>
<p>When I go through the DRep registration process, and include metadata
anchor information in the correct format</p>
<p>Then I will be able to register as a DRep via my wallet, GovTool will
include the metadata anchor in the registration certificate
transaction.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th>Confirm transaction has been sent</th>
<th><p>Given that I have gone through the DRep registration process</p>
<p>When I press the button on my wallet to submit the transaction</p>
<p>Then I will receive a confirmation message from GovTool that will
include a link to the transaction in a block explorer.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th>Status of transaction is displayed</th>
<th><p>Given that I have just submitted a DRep registration transaction,
and I am looking at the dashboard</p>
<p>When the registration has not yet been confirmed by the
blockchain,</p>
<p>Then the registration status will show as “In Progress” until it is
confirmed.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th rowspan="17">CH.VO4</th>
<th rowspan="17"><strong>As a DRep I want to vote</strong> so that I can
fulfil my role</th>
<th rowspan="4">Should be able to access the governance actions page as
a DRep with my wallet connected</th>
<th><p>Given that I am a DRep and I am connected to GovTool</p>
<p>When I visit the url of the governance actions page</p>
<p>Then the governance actions page is displayed</p></th>
<th></th>
<th></th>
<th rowspan="4">Voltaire</th>
<th rowspan="4">N</th>
</tr>
<tr class="header">
<th><p>Given that I am a DRep and connected to GovTool</p>
<p>When I look at the governance actions page</p>
<p>Then my voting power is displayed</p></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p>Given that I am a DRep and Connected to GovTool, and I am on the
governance actions page</p>
<p>When I click Disconnect Wallet</p>
<p>Then my wallet is disconnected and I am redirected to the same page,
but without the DRep functionality (i.e. ability to vote)</p></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p>Given that I am a DRep and I am on the governance actions
page</p>
<p>When I click on the “view proposal details” button</p>
<p>Then I will be shown the page for that individual governance action
and be able to view its details</p></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="4">A DRep should be able to vote on a live governance
action</th>
<th><p>Given that I am a DRep</p>
<p>When I look at the details page of an individual governance
action</p>
<p>Then I can see how many votes the governance action currently has
for, against and abstaining.</p></th>
<th></th>
<th></th>
<th rowspan="4">Voltaire</th>
<th rowspan="4">N</th>
</tr>
<tr class="header">
<th><p>Given that I am a DRep</p>
<p>When I look at the details page of an individual governance
action</p>
<p>Then there are buttons allowing me to vote for, against or
abstain.</p></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p>Given that I am a DRep, on the details page of an individual
governance action</p>
<p>When I select yes/ no/ abstain, and click vote</p>
<p>Then I can sign &amp; submit this vote via my wallet</p></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p>Given that I am a DRep</p>
<p>When I have submitted a vote</p>
<p>Then Immediately after this GovTool will display a message informing
me that my transaction has been sent and providing me with a link to a
block explorer where I can view the transaction</p></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th>People without the (t)ADA needed to pay for voting transactions
should not be able to submit a voting transaction</th>
<th><p>Given I have less Lovelace in my wallet than a transaction
costs</p>
<p>When I attempt to vote</p>
<p>The GovTool will tell me that there is an error</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th>People without their wallet connected or who do have their wallet
connected but have not registered as DReps should not be able to
vote</th>
<th><p>Given that I do not have a wallet connected to GovTool</p>
<p>When I visit the details of a governance action</p>
<p>Then I am not shown a vote button.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th>No one should be able to vote on a governance action that has
expired, or been ratified, or enacted.</th>
<th><p>Given that I am on the governance action page</p>
<p>When I examine the governance actions</p>
<p>None of the governance actions shown on the page have expired or been
ratified or enacted.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th rowspan="3">A DRep should be able to change their vote</th>
<th><p>Given that I am a DRep and I have already voted on a given
governance action</p>
<p>When I submit a different vote for the same transaction within the
same snapshot</p>
<p>Then the most recent vote will be counted.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th><p>Given that I have already cast a vote on a governance action</p>
<p>When I examine this specific governance action’s page</p>
<p>Then I can see that I have already voted and what my most recent vote
was</p></th>
<th></th>
<th></th>
<th></th>
<th>N</th>
</tr>
<tr class="header">
<th><p>Given that I have already cast a vote on a given governance
action</p>
<p>When I examine this specific governance action’s page</p>
<p>Then instead of seeing a “vote” button I should see a “change vote”
button</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th rowspan="2">Only the votes of participants who are still DReps at
the relevant epoch boundary will be accepted</th>
<th><p>Given that I am a DRep and I vote yes or abstain on a live
governance action.</p>
<p>At the epoch boundary</p>
<p>My votes are counted.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th><p>Given that I was a DRep that voted yes or abstain on a live
governance action but then retired.</p>
<p>At the next epoch boundary</p>
<p>My votes will not be counted towards the total tally of DRep
votes.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th>DReps can attach a metadata anchor to their votes</th>
<th><p>Given that I have chosen how to vote on the UI of a governance
action’s details</p>
<p>When I add a metadata anchor to the UI also and click the vote
button</p>
<p>Then the resulting transaction will include my metadata
anchor</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th rowspan="6">CH.VO5</th>
<th rowspan="6"><strong>As a DRep I want to retire</strong> so that I
can reclaim my DRep Deposit</th>
<th rowspan="2">Only a user who is registered as a DRep can retire</th>
<th><p>Given that I am not registered as a DRep,</p>
<p>When I look for a retirement option in GovTool</p>
<p>Then there is none.</p></th>
<th></th>
<th></th>
<th rowspan="2">Voltaire</th>
<th rowspan="2">N</th>
</tr>
<tr class="odd">
<th><p>Given that I am registered as a DRep,</p>
<p>When I look for a retirement option in GovTool there is one. And when
I choose this option</p>
<p>Then my wallet opens and I can sign a retirement action which is
registered on-chain.</p></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th>When I retire I get my deposit back</th>
<th><p>Given that I am a DRep</p>
<p>When I register a valid retirement transaction on chain</p>
<p>then my DRep registration deposit will be returned to me.</p></th>
<th></th>
<th></th>
<th></th>
<th>N</th>
</tr>
<tr class="odd">
<th rowspan="3">Only a user who has the wallet that they registered as a
DRep with can retire.</th>
<th><p>Given that I am not connected to GovTool</p>
<p>When I look at the homepage</p>
<p>Then I will not see an option to retire</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th><p>Given that I am connected to GovTool with an account that is not
associated with a registered DRep certificate</p>
<p>When I look at the homepage</p>
<p>Then I see an option to register as a DRep</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th><p>Given that I am a registered DRep with my wallet account
connected</p>
<p>When I click the retire as a DRep option on the homepage and then
send the retirement transaction with my wallet</p>
<p>Then the blockchain will register my retirement certificate, and I
will be retired.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th>CH.VO6</th>
<th><strong>As a DRep I want to update my details</strong> so that I can
better advertise myself to Ada Holders</th>
<th>A DRep can update their registration after registering</th>
<th><p>Given that I am a DRep and am connected to GovTool and am on the
dashboard.</p>
<p>Then when I click the “change metadata” button on the DRep tab.</p>
<p>Then I am directed to update my metadata and can submit a DRep update
certificate to register this on-chain.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th rowspan="11">CH.VO7</th>
<th rowspan="11">As any user <strong>I want to view governance
actions</strong> so I can see what is being proposed</th>
<th>Anyone should be able to access the governance actions page without
a wallet connected</th>
<th><p>Given that I am on the GovTool homepage,</p>
<p>When I click the “Governance actions” in the topbar</p>
<p>Then I am sent to the governance actions page.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th>I can see all live governance actions</th>
<th><p>Given that I am on the Governance Actions page</p>
<p>When I review the governance actions available to view on the
page,</p>
<p>Then all of the non expired/ ratified/enacted governance
actions.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th>Anyone with a CIP-95 compatible wallet connected should be able to
access the governance actions page</th>
<th><p>Given that I am on the GovTool dashboard,</p>
<p>When I click the View Governance Actions tab, or “Governance actions”
in the sidebar</p>
<p>Then I am sent to the governance actions page.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th>Should be able to see if a governance action has been accepted or
rejected by the Constitutional Committee</th>
<th><p>Given that I am looking at an individual governance action,</p>
<p>When I look at how many votes it has,</p>
<p>Then it shows the number of CC votes and whether this is
acceptance/veto or neither.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th rowspan="5">Should be able to view relevant information about
governance actions</th>
<th><p>Given that I am looking at a Treasury Withdrawal governance
action</p>
<p>Then I can see the amount of ADA that the proposal submitter wants to
withdraw, and the address that they want to withdraw it to.</p></th>
<th></th>
<th></th>
<th rowspan="5">Voltaire</th>
<th rowspan="5">N</th>
</tr>
<tr class="header">
<th><p>Given that I am looking at a Proposal Parameter Change governance
action,</p>
<p>Then I can see the parameter(s) that the Proposal Submitter is
proposing to change along with what the current values are, and what he
wants to change them to.</p></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p>Given that I am looking at a Constitutional Committee Update
governance action,</p>
<p>Then I can see the following (where applicable):<br />
- Old Committee Member Cold Key Hash to be removed<br />
- Float, (a rational number in the range from 0 to 1 inclusive. Of
course if all you have in a tool is Floats, than that is what it will
have to be)<br />
- Map of committee cold key credentials that will be added to the
committee with absolute epoch number number when they will
expire</p></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p>Given that I am looking at an Update to the Constitution
governance action</p>
<p>Then I should be able to see:<br />
- The Constitution URL<br />
- The Constitution hash<br />
- The proposal policy script (if provided when the governance action was
submitted)</p></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p>Given that I am looking at a Hard Fork Initiation governance
action</p>
<p>Then I should be able to see:<br />
- The new major protocol version</p></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th>The governance action as displayed should include a link to its
metadata</th>
<th><p>Given that I am reviewing the details of a specific governance
action</p>
<p>When I click on the “view other details” link on the governance
action details page</p>
<p>Then I will be shown a warning asking if I want to continue to an
external url (which will be displayed). If I continue then the external
url will open in a new tab.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th>Verify the integrity of a governance action’s metadata</th>
<th><p>Given that I am looking at a governance action</p>
<p>Then I can see whether a hash of that governance action’s metadata
matches the <em>metadata hash</em> included in the anchor.</p></th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th rowspan="4">CH.VO8</th>
<th rowspan="4">As a potential Constitutional Committee Member <strong>I
want to become a Constitutional Committee Member</strong> so that I can
vote on the corresponding governance actions</th>
<th>Create a set of keys</th>
<th>Given that I have the CLI open in front of me, when I run the
corresponding command, then I can verify that I have created a new key
pair</th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th>Include these keys in a New Committee Cold Key Hash or Script
Hash</th>
<th>Given that I am using CLI and I have created my set of keys, when
they are registered in the ledger, then I can verify that my set of keys
corresponds to a CC member</th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th>Create an authorization certificate</th>
<th>Given that I am using CLI and I have created my set of cold/hot key
pairs, when I run the corresponding command, then I can verify that the
certificate is stored on-chain and it delegates rights from the cold key
to the hot key</th>
<th></th>
<th></th>
<th><p>CIP-1694</p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/de76120a30552ef620d96401ed7fd3e5bca1f062/CIP-1694/README.md?plain=1#L993"><strong><u>L993</u></strong></a></p></th>
<th>N</th>
</tr>
<tr class="odd">
<th>Only votes from active Committee members are considered.</th>
<th>Given that my set of keys does not correspond to an active CC
member, when I try to vote as a CC member using CLI, then I get an error
message telling me that my credentials are not valid</th>
<th></th>
<th></th>
<th><p>CIP-1694</p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/de76120a30552ef620d96401ed7fd3e5bca1f062/CIP-1694/README.md?plain=1#L993"><strong><u>L993</u></strong></a></p></th>
<th>N</th>
</tr>
<tr class="header">
<th rowspan="5">CH.VO9</th>
<th rowspan="5"><strong>As a CC Member I want to review a governance
action</strong> so that I can scrutinise whether or not it is aligned
with the Constitution</th>
<th><p>Access GovTool</p></th>
<th>Given that I am on the GovTool homepage, when I click the
“Governance actions” in the topbar then I am sent to the governance
actions page.</th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th>See list of current governance actions</th>
<th>Given that I am on the Governance Actions page When I review the
governance actions available to view on the page, then all of the non
expired/ ratified/enacted governance actions.</th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th>See details of a specific governance action</th>
<th>Given that I am on the Governance Actions page, When I click on an
individual governance action, Then I can see the relevant
information</th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th>See metadata</th>
<th>Given that I am looking at an individual governance action page,
when I click on “view other details” and I click on continue in the
warning message, Then an external url will open in a new tab.</th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th>Verify metadata integrity</th>
<th>Given that I am looking at a governance action then I can see
whether a hash of that governance action’s metadata matches the metadata
hash included in the anchor.</th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th rowspan="5">CH.VO10</th>
<th rowspan="5"><strong>As a CC Member I want to vote on a governance
action</strong> so that I can approve governance actions that align with
the constitution</th>
<th><p>Find a specific governance action using CLI</p></th>
<th>Given that I am using CLI and I know the governance action ID, When
I run the command to review a specific governance action, Then I can see
the details of that individual governance action.</th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th rowspan="2">Vote as a Constitutional Committee member using CLI</th>
<th>Given that I am using CLI and I know the governance action ID, When
I build the transaction to vote on a governance action, Then I can
specify my role (ccm), the action ID, and the intent to vote
(YES/NO/ABSTAIN)</th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th>Given that I am using CLI and I have built the transaction to vote
on a specific governance action, When I run the command to sign the
transaction, Then I can submit the transaction and pay the transaction
costs</th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th><p>Provide rationale for vote with a metadata anchor</p></th>
<th>Given that I am using CLI, When I am building a transaction to vote
on a specific governance action, Then I can use the metadata anchor to
provide a rationale for my vote</th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th>Change vote</th>
<th>Given that I have submitted a vote on a specific governance action,
When I vote again on the same governance action, Then I can change the
intent to vote (YES/NO/ABSTAIN)</th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th>CH.VO11</th>
<th><strong>As a CC Member I want to change my voting
credentials</strong> so I can manage my organisation’s voting</th>
<th>Create a new authorization certificate</th>
<th>Given that I am a CC member and I have enough funds to pay the
transaction fees, When I create a new authorisation certificate using
the same cold key, Then a new hot key is authorised to vote as a valid
CC member</th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="odd">
<th>CH.VO12</th>
<th><strong>As a CC Member I want to retire</strong> so my credentials
are no longer valid</th>
<th>Create a resignation certificate</th>
<th>Given that I am a CC member and I have enough funds to pay the
transaction fees, When I create a resignation certificate, Then my cold
key and the derived hote keys are no longer valid to vote as a CC
member</th>
<th></th>
<th></th>
<th>Voltaire</th>
<th>N</th>
</tr>
<tr class="header">
<th>CH.CLI1</th>
<th><strong>As a Plutus developer I want the Node to support Plutus V3
requirements for CIP-1694</strong></th>
<th><p><em>Correct operation of BLS primitives.</em></p>
<p><em>Correct operation of new bitwise primitives.</em></p>
<p><em>New Plutus V3 cost model is used correctly for the new
primitives.</em></p>
<p><em>Plutus scripts are correctly used for DRep voting.</em></p>
<p><em>Plutus scripts on the constitution correctly control CC
voting.</em></p>
<p><em>Benchmark execution times are within acceptable
range.</em></p></th>
<th>Detail pending</th>
<th></th>
<th>Detail pending</th>
<th>API/CLI</th>
<th></th>
</tr>
<tr class="odd">
<th>CH.API11</th>
<th><strong>Ledger API User Story</strong></th>
<th>This is a placeholder</th>
<th>Detail pending</th>
<th></th>
<th></th>
<th>API/CLI</th>
<th>UPDATE/REMOVE</th>
</tr>
<tr class="header">
<th>VO16</th>
<th><strong>SPO Interface User Story</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th>API/CLI</th>
<th>UPDATE/REMOVE</th>
</tr>
<tr class="odd">
<th>INT1</th>
<th>As a user of the system I want governance actions to be correctly
submitted on chain</th>
<th></th>
<th>Detail pending</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><em>INT2</em></th>
<th><em>As a user of the system I want All actions to be ratified
on-chain correctly according to the CIP-1694 rules</em></th>
<th><em>(voter type, thresholds, DRep activity)</em></th>
<th>Detail pending</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="2"><em>INT3</em></th>
<th rowspan="2"><em>As a user of the system I want All governance
actions to be enacted on time on-chain following ratification</em></th>
<th><strong>Timely</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><strong>Correctly according to CIP-1694
rules:</strong><em>Parameter updates, Info, Hard Forks, No Confidence,
New Committee, New Constitution, Treasury Withdrawals. This will expand
into many requirements.</em></p></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th colspan="8"><strong>SYSTEM LEVEL (not fully completed
yet)</strong></th>
</tr>
<tr class="header">
<th><a
href="https://docs.google.com/document/d/1Ymj_Foh3lVYq2asI5WEdQYBud5B8KbJcw4jpUwuv5p8/edit#bookmark=id.yzo1aziuwsxs"><u>CIP1</u></a></th>
<th><p><strong>As</strong> any persona</p>
<p><strong>I want</strong> the hash value of the off-chain Constitution
to be recorded on-chain</p>
<p><strong>So that</strong> I can verify the authenticity of the
off-chain document</p></th>
<th>Hash value of the off-chain Constitution is recorded on-chain</th>
<th>Given that I access a Cardano Explorer and that it display the
ledger states accurately, Then I can access a map of the current
constitution hash and the URL of the off-chain document</th>
<th></th>
<th><strong>Detail Pending</strong></th>
<th><p>CIP-1694</p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/de76120a30552ef620d96401ed7fd3e5bca1f062/CIP-1694/README.md?plain=1#L958C19-L958C120"><strong><u>L958</u></strong></a></p></th>
<th></th>
</tr>
<tr class="odd">
<th><a
href="https://docs.google.com/document/d/1Ymj_Foh3lVYq2asI5WEdQYBud5B8KbJcw4jpUwuv5p8/edit#bookmark=id.elqu6qa8ltse"><u>CIP2</u></a></th>
<th><p><strong>As</strong> an ada holder</p>
<p><strong>I want</strong> the key hash of active and expired Committee
Members and their terms to be registered on-chain</p>
<p><strong>So that</strong> the system can count their votes</p></th>
<th><p>Committee members key hashes must be recorded on chain and be
publicly accessible</p>
<p>ADA holder must be able to check that the key hashes of active and
expired committee members are registered on-chain status</p></th>
<th>Given that the node is up to date, then it should include a record
for each committee member detailing their key-hashes, term information
(end epochs), and the corresponding cold to hot key authorization
maps.</th>
<th></th>
<th><strong>Detail Pending</strong></th>
<th><p>CIP-1694</p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/de76120a30552ef620d96401ed7fd3e5bca1f062/CIP-1694/README.md?plain=1#L993"><strong><u>L993</u></strong></a></p></th>
<th></th>
</tr>
<tr class="header">
<th><a
href="https://docs.google.com/document/d/1Ymj_Foh3lVYq2asI5WEdQYBud5B8KbJcw4jpUwuv5p8/edit#bookmark=id.pddqksyfshgc"><u>CIP3</u></a></th>
<th><p><strong>As an</strong> ada holder</p>
<p><strong>I want</strong> to be able to submit a proposal to replace
all or part of the current constitutional committee</p>
<p><strong>So that</strong> committee members that have lost confidence
of ada holders can be removed from their duties.</p></th>
<th><p>It must be possible to replace the constitutional committee via a
governance action</p></th>
<th><p>Any ada holder can submit a governance action that proposes to
add or remove one or many new committee members.</p>
<p>Given that a governance action to update the committee has been
proposed And both SPO and DRep YES votes are equal or greater than the
required threshold (depending on state of no-confidence or normal
state)</p>
<p>The governance action is ratified and enacted automatically at the
next epoch transition, otherwise it’s expired.</p></th>
<th></th>
<th><strong>Detail Pending</strong></th>
<th><p>CIP-1694</p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/de76120a30552ef620d96401ed7fd3e5bca1f062/CIP-1694/README.md?plain=1#L997C1-L997C78"><strong><u>L997</u></strong></a></p></th>
<th></th>
</tr>
<tr class="odd">
<th><a
href="https://docs.google.com/document/d/1Ymj_Foh3lVYq2asI5WEdQYBud5B8KbJcw4jpUwuv5p8/edit#bookmark=id.mca6cvcoht53"><u>CIP4</u></a></th>
<th><p><strong>As an</strong> ada holder</p>
<p>I want the size of the constitutional committee</p>
<p>To be not-fixed</p>
<p>So that I can propose a different size via a governance
action</p></th>
<th>Size of the constitutional committee must be variable</th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th><strong>Detail Pending</strong></th>
<th><a
href="https://github.com/cardano-foundation/CIPs/blob/ada2cf6a9e27fbdf37ca1be0780371fbab2b7748/CIP-1694/README.md?plain=1#L1009"><strong><u>L1009</u></strong></a></th>
<th></th>
</tr>
<tr class="header">
<th><a
href="https://docs.google.com/document/d/1Ymj_Foh3lVYq2asI5WEdQYBud5B8KbJcw4jpUwuv5p8/edit#bookmark=id.tdyxk950f5v8"><u>CIP5</u></a></th>
<th><p>As an ada holder,</p>
<p>I want that the committee threshold (the fraction of committee is not
fixed</p>
<p>So that I can propose a different threshold via a governance
action</p></th>
<th><strong>Size of</strong> committee threshold must be variable</th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th><strong>Detail Pending</strong></th>
<th><a
href="https://github.com/cardano-foundation/CIPs/blob/ada2cf6a9e27fbdf37ca1be0780371fbab2b7748/CIP-1694/README.md?plain=1#L1011"><strong><u>L1011</u></strong></a></th>
<th></th>
</tr>
<tr class="odd">
<th>CIP6</th>
<th><p>As an ada holder</p>
<p>I want to be able to have elect an empty committee if the community
wishes to abolish the constitutional committee entirely</p>
<p>So that SPO and Dreps can continue to ratify governance actions
without the need of a constitutional committee</p></th>
<th><p>Users must be able to elect an empty committee</p>
<p>Ratifying governance actions must be possible without constitutional
committee</p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th><strong>Detail Pending</strong></th>
<th><a
href="https://github.com/cardano-foundation/CIPs/blob/ada2cf6a9e27fbdf37ca1be0780371fbab2b7748/CIP-1694/README.md?plain=1#L1014"><strong><u>L1014</u></strong></a></th>
<th></th>
</tr>
<tr class="header">
<th>CIP7</th>
<th><p><strong>As</strong> an Ada holder,</p>
<p><strong>I want</strong> to submit a governance action,</p>
<p><strong>So that</strong> it can be considered by the governance
bodies/process.</p></th>
<th><p><strong>There must be a command in in the Cardano CLI allowing
the user to submit a governance action</strong></p>
<p>The input must include validation checks for format and criteria</p>
<p>After successful validation the</p>
<p>user must be informed of confirmation through the CLI</p>
<p>An action should have an accepted or rejected status?</p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th><strong>Detail Pending</strong></th>
<th>CIP-1694</th>
<th></th>
</tr>
<tr class="odd">
<th>CIP8</th>
<th><p><strong>As</strong> a delegate representative (DRep),</p>
<p><strong>I want</strong> to vote on submitted governance actions,</p>
<p><strong>So that</strong> I can represent the interests of my
delegates.</p></th>
<th><p>DReps must have access to the list of current governance actions
(can we specify where they get it?).</p>
<p>DReps should be able to cast their vote on each action (through the
CL or through an app)?</p>
<p>An action should have an accepted or rejected status?</p></th>
<th><p>Given that a Drep has casted a vote the system accurately records
and reflects these votes.</p></th>
<th></th>
<th><strong>Detail Pending</strong></th>
<th>CIP-1694</th>
<th></th>
</tr>
<tr class="header">
<th>CIP9</th>
<th><p><strong>As</strong> an Ada holder,</p>
<p><strong>I want</strong> to view the status of governance actions,</p>
<p><strong>So that</strong> I am informed about the governance
process.</p></th>
<th><p>Users must be able to view a list of governance actions with
their current status.</p>
<p>The status must include stages like submission, voting, ratification,
timeline.</p>
<p>The system must provide real-time updates on the status.</p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th><strong>Detail Pending</strong></th>
<th>CIP-1694</th>
<th></th>
</tr>
<tr class="odd">
<th>CIP10</th>
<th><p><strong>As</strong> an Ada holder,</p>
<p><strong>I want</strong> to delegate my voting rights to a DRep,</p>
<p><strong>So that</strong> my interests are represented in the
governance process.</p></th>
<th><p>ADA holders can select a DRep to delegate their voting
rights.</p>
<p>The delegation process should be user-friendly and must be
secure.</p>
<p>The system must confirms successful delegation.</p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th>CIP11</th>
<th><p><strong>As</strong> an SPO,</p>
<p><strong>I want</strong> to participate in the governance voting,</p>
<p><strong>So that</strong> I can contribute to the decision-making
process.</p></th>
<th><p>SPOs must have access to governance actions for voting.</p>
<p>SPOs can cast their votes based on the ADA staked in their pools.</p>
<p>The system accurately reflects the votes of SPOs.</p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th colspan="8"><strong>CARDANO CLI US</strong></th>
</tr>
<tr class="header">
<th>CLI01</th>
<th><p><strong>As</strong> an Ada holder,</p>
<p><strong>I want</strong> to obtain the hash of the off-chain text of a
Constitution</p>
<p><strong>So that</strong> I can compare it against the hash registered
on-chain to verify its authenticity.</p></th>
<th>When I provide the off-chain text of the Constitution, the
cardano-cli should calculate and return the corresponding blake2b-256
hash of the document.</th>
<th><p>Given that a holder provides the offchain text of the
constitution then cardo-cli should return the corresponding blake2b-256
hash</p>
<p>Given that it is the same document, the resulting hash should match
the one registered on-chain.</p></th>
<th></th>
<th></th>
<th><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L958"><u>L958</u></a></th>
<th></th>
</tr>
<tr class="odd">
<th>CLI02</th>
<th><p><strong>As</strong> an Ada holder,</p>
<p><strong>I want</strong> to generate the hash of the off-chain text
for a proposed Constitution</p>
<p><strong>So that</strong> the hash can be utilized in a governance
action.</p></th>
<th>When I provide the off-chain text of the Constitution, the
cardano-cli should calculate and return the corresponding blake2b-256
hash of the document.</th>
<th><p>Given that a holder provides the offchain text of the
constitution then cardo-cli should return the corresponding blake2b-256
hash</p>
<p>Given that it is the same document, the resulting hash should match
the one registered on-chain.</p></th>
<th></th>
<th></th>
<th><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L958"><u>L958</u></a></th>
<th></th>
</tr>
<tr class="header">
<th rowspan="8">CLI03</th>
<th rowspan="8"><p><strong>As</strong> a potential Constitutional
Committee member,</p>
<p><strong>I want</strong> to generate COLD key pair</p>
<p><strong>So that</strong> I can be proposed for the Committee in a
Governance action</p></th>
<th><mark>The feature implementation should include a new command:<br />
<br />
cardano-cli conway governance committee key-gen-cold</mark></th>
<th>Typing <mark>cardano-cli conway governance committee key-gen-cold
with accepted input parameters generates a COLD key pair. If a parameter
or the command format is incorrect an error is raised</mark></th>
<th></th>
<th></th>
<th><p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L966C33-L966C52"><u>L966</u></a></p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></p></th>
<th></th>
</tr>
<tr class="odd">
<th>Includes a corresponding CLI usage describing the feature, how to
use it and the types of the inputs and outputs.</th>
<th>Typing <mark>cardano-cli conway governance committee key-gen-cold
—-help displays command usage</mark></th>
<th></th>
<th></th>
<th><p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L966C33-L966C52"><u>L966</u></a></p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></p></th>
<th></th>
</tr>
<tr class="header">
<th><p>The command must accept two flags</p>
<p>--cold-verification-key-file</p>
<p>--cold-signing-key-file</p></th>
<th>Both flags are mandatory and each produces the corresponding
verification or signing key file</th>
<th></th>
<th></th>
<th><p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L966C33-L966C52"><u>L966</u></a></p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></p></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The generated key pair should be stored in the specified
files:</mark></p>
<p><mark>the verification key is saved in the file specified by</mark>
--cold-verification-key-file</p>
<p> <mark>the signing key saved in the file specified by</mark></p>
<p>--cold-signing-key-file</p></th>
<th>Given that the user specifies a valid path and file name, Then the
keys are saved on that file and location.</th>
<th></th>
<th></th>
<th><p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L966C33-L966C52"><u>L966</u></a></p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></p></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The generated keys should adhere to text envelope format used
for other credentials</mark></th>
<th>Given that the cli has created the verification and signing keys,
then these conform to the text envelope format used consisting of a json
object with type, description and cborhex fields.</th>
<th></th>
<th></th>
<th><p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L966C33-L966C52"><u>L966</u></a></p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></p></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The signing key text envelope contains the correct type,
description, and CBOR value.</mark></p>
<p><mark><strong>Type</strong>
"ConstitutionalCommitteeColdSigningKey_ed25519"</mark></p>
<p><strong><mark>Description</mark></strong></p>
<p><mark>"Constitutional Committee Cold Signing Key"</mark></p></th>
<th><p>Given that the signing key is saved on a text envelope format,
the type and description fields are:</p>
<p><mark><strong>Type</strong>
"ConstitutionalCommitteeColdSigningKey_ed25519"</mark></p>
<p><strong><mark>Description</mark></strong></p>
<p><mark>"Constitutional Committee Cold Signing Key"</mark></p></th>
<th></th>
<th></th>
<th><p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L966C33-L966C52"><u>L966</u></a></p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></p></th>
<th></th>
</tr>
<tr class="header">
<th><p>The verification key text envelope has:</p>
<p><strong>Type</strong>
"CConstitutionalCommitteeColdVerificationKey_ed25519"</p>
<p><strong>Description</strong></p>
<p>"Constitutional Committee Cold Verification Key"</p></th>
<th><p>Given that the verification key is saved on a text envelope
format, the type and description fields are:</p>
<p><strong>Type</strong>
<mark>"CConstitutionalCommitteeColdVerificationKey_ed25519"</mark></p>
<p><strong>Description</strong></p>
<p><mark>"Constitutional Committee Cold Verification
Key"</mark></p></th>
<th></th>
<th></th>
<th><p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L966C33-L966C52"><u>L966</u></a></p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></p></th>
<th></th>
</tr>
<tr class="odd">
<th><p>Failing to provide a file name for any of</p>
<p>--cold-verification-key-file</p>
<p>--cold-signing-key-file</p>
<p>fails with an appropriate error message.</p></th>
<th><p><strong>Given</strong> the user has not inputed either
<mark>--cold-verification-key-file</mark> OR</p>
<p><mark>--cold-signing-key-file</mark> parameters <strong>THEN</strong>
the command fails and returns an error to the users informing them to
fill those parameters in. The error message should prompt the user to
consult the command usage (--help)</p></th>
<th></th>
<th></th>
<th><p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L966C33-L966C52"><u>L966</u></a></p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></p></th>
<th></th>
</tr>
<tr class="header">
<th rowspan="8">CLI04</th>
<th rowspan="8"><p><strong>As</strong> potential Constitutional
Committee member,</p>
<p><strong>I want</strong> to generate HOT key pair</p>
<p><strong>So that</strong> I can authorise the Hot key to sign votes on
behalf of the Cold key</p></th>
<th><mark>The feature implementation should include a new command:<br />
<br />
cardano-cli conway governance committee key-gen-hot</mark></th>
<th><p>Given that a potential constitutional committee member has
entered the <mark>cardano-cli conway governance committee key-gen-hot
command with all the required and correct parameters</mark> then the
command is executed successfully and a HOT key pair is generated.</p>
<p><mark>If a parameter or the command format is incorrect an error is
raised</mark></p></th>
<th></th>
<th></th>
<th><p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L966C33-L966C52"><u>L966</u></a></p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></p></th>
<th></th>
</tr>
<tr class="odd">
<th>Includes a corresponding CLI usage describing the feature, how to
use it and the types of the inputs and outputs.</th>
<th>Typing <mark>cardano-cli conway governance committee key-gen-hot
displays command usage</mark></th>
<th></th>
<th><strong>Detail Pending</strong></th>
<th><p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L966C33-L966C52"><u>L966</u></a></p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></p></th>
<th></th>
</tr>
<tr class="header">
<th><p>The command must accept two flags</p>
<p>--verification-key-file</p>
<p>--signing-key-file</p></th>
<th>Both flags are mandatory and each produces the corresponding
verification or signing key file</th>
<th></th>
<th><strong>Detail Pending</strong></th>
<th><p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L966C33-L966C52"><u>L966</u></a></p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></p></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The generated key pair should be stored in the specified
files:</mark></p>
<p><mark>the verification key saved in the file specified by</mark></p>
<p><mark>--verification-key-file</mark></p>
<p><mark>the signing key saved in the file specified by</mark></p>
<p><mark>--signing-key-file</mark></p></th>
<th>Given that the user specifies a valid path and file name, Then the
keys are saved on that file and location.</th>
<th></th>
<th></th>
<th><p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L966C33-L966C52"><u>L966</u></a></p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></p></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The generated keys should adhere to text envelope format used
for other credentials</mark></th>
<th>Given that the cli has created the verification and signing keys,
then these conform to the text envelope format used consisting of a json
object with type, description and cbor hex fields.</th>
<th></th>
<th></th>
<th><p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L966C33-L966C52"><u>L966</u></a></p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></p></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The <strong>signing</strong> key text envelope contains the
correct type, description, and CBOR value.</mark></p>
<p><mark><strong>Type</strong>
"ConstitutionalCommitteeColdSigningKey_ed25519"</mark></p>
<p><strong><mark>Description</mark></strong></p>
<p><mark>"Constitutional Committee Cold Signing Key"</mark></p></th>
<th><p>Given that the signing key is saved on a text envelope format,
the type and description fields are:</p>
<p><strong><mark>Type</mark></strong>
"ConstitutionalCommitteeColdSigningKey_ed25519"</p>
<p><strong><mark>Description</mark></strong></p>
<p>"Constitutional Committee Cold Signing Key"</p></th>
<th></th>
<th></th>
<th><p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L966C33-L966C52"><u>L966</u></a></p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></p></th>
<th></th>
</tr>
<tr class="header">
<th><p>The <strong>verification</strong> key text envelope has:</p>
<p><strong>Type<br />
</strong>"CConstitutionalCommitteeColdVerificationKey_ed25519"</p>
<p><strong>Description<br />
</strong>"Constitutional Committee Cold Verification Key"</p></th>
<th><p>Given that the verification key is saved on a text envelope
format, the type and description fields are:</p>
<p><strong>Type<br />
</strong>"CConstitutionalCommitteeColdVerificationKey_ed25519"</p>
<p><strong>Description<br />
</strong>"Constitutional Committee Cold Verification Key"</p></th>
<th></th>
<th></th>
<th><p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L966C33-L966C52"><u>L966</u></a></p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></p></th>
<th></th>
</tr>
<tr class="odd">
<th><p>Failing to provide a file name for any of the flags</p>
<p>--verification-key-file</p>
<p>--signing-key-file</p>
<p>fails with an appropriate error message.</p></th>
<th><p><strong>Given</strong> the user has not inputted either
--verification-key-file OR</p>
<p>--signing-key-file parameters <strong>THEN</strong> the command fails
and returns an error to the users informing them to fill those
parameters in. The error message should prompt the user to consult the
command usage (--help)</p></th>
<th></th>
<th></th>
<th><p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L966C33-L966C52"><u>L966</u></a></p>
<p><a
href="https://github.com/cardano-foundation/CIPs/blob/d6c5ad3a77b4684bc19f3cafb75b4886a67c9a31/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></p></th>
<th></th>
</tr>
<tr class="header">
<th rowspan="9">CLI05</th>
<th rowspan="9"><p>As a committee member</p>
<p>I want to issue a authorization certificate from my cold key to a hot
key</p>
<p>So that I can sign my votes using the hot key and keep the cold key
in cold storage and can authorise a new hot key in case the original one
is compromised.</p></th>
<th><p><mark>The feature implementation should include a new command in
the cardano-cli:</mark></p>
<p><mark>cardano-cli conway governance committee
create-hot-key-authorization-certificate</mark></p></th>
<th>Typing <mark>cardano-cli conway governance committee
create-hot-key-authorization-certificate with accepted input parameters
generates a hot key authorization certificate. If a parameter or the
command format is incorrect an error is raised</mark></th>
<th></th>
<th></th>
<th><a
href="https://github.com/cardano-foundation/CIPs/blob/0f64c52fe1350b4e93c23f6bced92d4ca576538e/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></th>
<th></th>
</tr>
<tr class="odd">
<th><p>The command should accept the necessary flags:</p>
<p>--cold-verification-key, --cold-verification-key-file,
--cold-verification-key-hash, --hot-verification-key,
--hot-verification-key-file, --hot-verification-key-hash, and
--out-file.</p></th>
<th><p>The command allows passing credentials as follows</p>
<p>Cold verification key &lt;- string</p>
<p>Cold verification key file &lt;- file</p>
<p>Cold verification key hash &lt;- string</p>
<p>Hot verification key &lt;- string</p>
<p>Hot verification key file &lt;- file</p>
<p>Hot verification key hash &lt;- string<br />
<br />
Failing to provide the right input results in a clear error message that
helps the user to identify the problem</p></th>
<th></th>
<th></th>
<th><a
href="https://github.com/cardano-foundation/CIPs/blob/0f64c52fe1350b4e93c23f6bced92d4ca576538e/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></th>
<th></th>
</tr>
<tr class="header">
<th><mark>Running the command with the appropriate flags should generate
a hot key authorization certificate and be saved in the specified output
file.</mark></th>
<th>Given that the user specifies a valid path and file name, then the
command produces a Cold to Hot authorization certificate on the right
location and name.</th>
<th></th>
<th></th>
<th><a
href="https://github.com/cardano-foundation/CIPs/blob/0f64c52fe1350b4e93c23f6bced92d4ca576538e/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The hot key authorization certificate should follow the
text envelope format of other existing certificates, including the type,
description, and CBOR hex value.</mark></p>
<p><mark>{</mark></p>
<p> <mark>"type": "CertificateConway",</mark></p>
<p> <mark>"description": "Constitutional Committee Hot Key Authorization
Certificate",</mark></p>
<p> <mark>"cborHex": ""</mark></p>
<p><mark>}</mark></p></th>
<th>Given that the authorization certificate is saved, then it is in a
text envelope format consisting of a json object with type, description
and cbor hex fields.</th>
<th></th>
<th></th>
<th><a
href="https://github.com/cardano-foundation/CIPs/blob/0f64c52fe1350b4e93c23f6bced92d4ca576538e/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></th>
<th></th>
</tr>
<tr class="header">
<th>The type of the certificate should be: "CertificateConway"</th>
<th>The type field ont the text envelope of the certificate is<br />
"CertificateConway"</th>
<th></th>
<th></th>
<th><a
href="https://github.com/cardano-foundation/CIPs/blob/0f64c52fe1350b4e93c23f6bced92d4ca576538e/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The description of the certificate should be:</mark></p>
<p><mark>"Committee HotKey Authorization Certificate"</mark></p></th>
<th>The description field on the text envelope of the certificate
is<br />
<mark>"Committee HotKey Authorization Certificate"</mark></th>
<th></th>
<th></th>
<th><a
href="https://github.com/cardano-foundation/CIPs/blob/0f64c52fe1350b4e93c23f6bced92d4ca576538e/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The certificate must comply with the cddl:</mark></p>
<p> <mark>auth_committee_hot_cert = (14, committee_cold_credential,
committee_hot_credential)</mark></p></th>
<th><p>Given that the authorization certificate is saved,then it is on
the form of a text envelope consisting of a json object with type,
description and cbor hex fields , where</p>
<p>Cbor hex conforms to the authorization certificate as defined on the
cddl</p>
<p><mark>auth_committee_hot_cert = (14, committee_cold_credential,
committee_hot_credential)</mark></p></th>
<th></th>
<th></th>
<th><a
href="https://github.com/cardano-foundation/CIPs/blob/0f64c52fe1350b4e93c23f6bced92d4ca576538e/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></th>
<th></th>
</tr>
<tr class="odd">
<th>The command should handle potential errors, such as missing or
invalid flags, and provide appropriate error messages indicating the
missing or required parameters.</th>
<th>The command should handle potential errors, such as missing or
invalid flags, and provide appropriate error messages indicating the
missing or required parameters.</th>
<th></th>
<th></th>
<th><a
href="https://github.com/cardano-foundation/CIPs/blob/0f64c52fe1350b4e93c23f6bced92d4ca576538e/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></th>
<th></th>
</tr>
<tr class="header">
<th>Documentation should be provided, including a corresponding CLI
usage, describing the feature, its purpose, and how to use it, along
with the expected types of inputs and outputs.</th>
<th>Typing <mark>cardano-cli conway governance committee
create-hot-key-authorization-certificate —-help displays command
usage</mark></th>
<th></th>
<th></th>
<th><a
href="https://github.com/cardano-foundation/CIPs/blob/0f64c52fe1350b4e93c23f6bced92d4ca576538e/CIP-1694/README.md?plain=1#L993"><u>L993</u></a></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="6">CLI06</th>
<th rowspan="6"><p>As a potential constitutional committee member</p>
<p>I want to generate the key hashes for my cold and hot keys</p>
<p>So that they can be used by third parties to propose me as a new
committee member and for identification purposes once Ive been elected
as committee member</p></th>
<th><p><mark>The command generates the blake2b 256 hash of the
verification key</mark></p>
<p><mark>cardano-cli conway governance committee
key-hash</mark></p></th>
<th>Typing <mark>cardano-cli conway governance committee key-hash with
accepted input parameters generates blake2b 256 hash of the verification
key. If a parameter or the command format is incorrect an error is
raised</mark></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p>Accepts the flags</p>
<p><mark>--verification-key</mark>
<mark>--verification-key-file</mark></p>
<p>To provide the verification key.</p></th>
<th>Both flags are mandatory and each produces the corresponding
verification or signing key file</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command gives the option –out-file.</mark> If the
--out-file flag is provided, the key hash should be saved to the
specified file.</th>
<th>Given that the user specifies the <mark>–out-file parameter
and</mark> a valid path and file name, Then the key hash is saved on
that file and location.</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th>If the --out-file flag is not provided, the key hash should be
printed to the standard output (stdout) in a readable format.</th>
<th>Given that the user has not specified the <mark>–out-file parameter
then the key hash must returned in clear text through stdout (cmd
output)</mark></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th>The command should handle potential errors, such as missing flags or
invalid input, and provide appropriate error messages or exceptions to
guide the user.</th>
<th>Given that the user has executed the correct command but has either
filled incorrectly any of the parameters, missed any mandatory flag
and/or parameter then an exception should be raised and an error message
should be returned with clear indication as to how to fix the issue.
When not feasible, the user should be directed to the usage page of the
command (<mark>cardano-cli conway governance committee key-hash</mark>
--help)</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th>Documentation should be provided, including a corresponding CLI
usage, describing the feature, its purpose, and how to use it, along
with the expected types of inputs and outputs.</th>
<th>Typing <mark>cardano-cli conway governance committee key-hash</mark>
--help display the command usage page</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="10">CLI07</th>
<th rowspan="10"><p>As a constitutional committee member</p>
<p>I want to be able to generate a resignation certificate</p>
<p>So that i can submit it it to the chain on a transaction to signal to
the ada holders that I’m resigning from my duties as cc member</p></th>
<th>The command should be implemented in the cardano-cli as cardano-cli
governance committee create-cold-resignation-certificate</th>
<th>Typing cardano-cli governance committee
create-cold-resignation-certificate with accepted input parameters
generates a cold resignation certificate.</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p>The command should accept the following ways to supply
credentials: cold verification key file, the cold verification key or
the cold verification key hash so it accepts the following flags:</p>
<p>--cold-verification-key,</p>
<p>--cold-verification-key-file,</p>
<p>--cold-verification-key-hash.</p></th>
<th><p>The command allows passing credentials as follows</p>
<p>Cold verification key &lt;- string</p>
<p>Cold verification key file &lt;- file</p>
<p>Cold verification key hash &lt;- string</p>
<p>If any of the inputs has the wrong format the cli raises an arrow
message indicating the missing or incorrect parameter.</p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th>The command allows an optional anchor (url/hash) for the
resigning<br />
cc member to express their<br />
motivation for resigning.</th>
<th><p>The command allows for an OPTIONAL anchor comprised of a URL
containing a document where the resigning CC member expresses the
motivations and the hash of the document</p>
<p>The CLI does not check for the validity of the URL, the contents, or
that the documents and declared hash match.</p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th> The resignation certificate should be saved in the specified output
file using the --out-file flag.</th>
<th>Given that the CC member issuing the resignation certificate
provides a valid path and file name, then the certificate is saved on
the specified location.</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p>The generated resignation certificate should be consistent with
the text envelope format of existing certificates in Cardano, including
the specified JSON structure with the correct type, description, and
CBOR-encoded value.</p>
<p>{</p>
<p> "type": "CertificateConway",</p>
<p> "description": "Constitutional Committee Cold Key Resignation
Certificate",</p>
<p> "cborHex": ""</p>
<p>}</p></th>
<th>Given that the resignation certificate is saved, then it is in a
text envelope format consisting of a json object with type, description
and cbor hex fields.</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th>The certificate type should be ConwayResignCommitteeColdKey to
indicate a resignation of the Committee Cold Key.</th>
<th>Given that the certificate is in a text envelope format, then its
type is<br />
<br />
Type: ConwayResignCommitteeColdKey</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p>The certificate description should be</p>
<p>"description": "Constitutional Committee Cold Key Resignation
Certificate"</p></th>
<th>Given that the certificate is in a text envelope format, then its
description field is<br />
<br />
"description": "Constitutional Committee Cold Key Resignation
Certificate"</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p> The command should generate a resignation certificate according
to the conway cddl:</p>
<p><strong>resign_committee_cold_cert = (15, committee_cold_credential,
anchor / null)</strong></p></th>
<th><p>Given that the certificate is in a text envelope format, then its
cbor hex field conforms to the conway cddl</p>
<p><strong>resign_committee_cold_cert = (15, committee_cold_credential,
anchor / null)</strong></p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th>The command should handle potential errors, such as missing or
invalid flags or keys, and provide appropriate error messages indicating
the missing or required parameters.</th>
<th>If any required input parameter is missing or incorrect, the command
should raise an error indicating the missing or incorrect
parameter.</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p>Documentation should be provided, including a corresponding CLI
usage, describing the feature, its purpose, and how to use it, along
with the expected types of inputs and outputs.</p></th>
<th>Given that the user has executed the correct command but has either
filled incorrectly any of the parameters, missed any mandatory flag
and/or parameter then an exception should be raised and an error message
should be returned with clear indication as to how to fix the issue.
When not feasible, the user should be directed to the usage page of the
command (<mark>cardano-cli governance committee
create-cold-resignation-certificate</mark> --help)</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="5">CLI08</th>
<th rowspan="5"><p>As an ada holder</p>
<p>I want to generate Ed25519 keys</p>
<p>So that I can register as a DRep</p></th>
<th>The command is implemented as<br />
<br />
cardano-cli conway governance drep key-gen</th>
<th>Typing cardano-cli conway governance drep key-gen with accepted
input parameters generates an Ed25519 key pair</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th>The command supports the --verification-key-file FILE option to
specify the file where the generated verification key will be
saved.</th>
<th>The flag --verification-key-file is mandatory,</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th>The command supports the --signing-key-file FILE option to specify
the file where the generated signing key will be saved. File is saved on
the specified path</th>
<th>The flag --signing-key-file is mandatory,</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>When the command is executed, it generates both the
verification key and signing key</mark> File is saved on the specified
path</th>
<th><p>Given that the user specifies valid paths and file names then,
the corresponding verification and signing key files are saved on the
paths specified by the user.</p>
<p>If the paths do not exist or are inaccessible, an error message is
raised.</p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p>The key generation should follow the current design for key
generation and output in an envelope format.</p></th>
<th><p>Given that the verification and signing key files are saved, then
they are in a text envelope format consisting of a json object with
type, description and cbor hex fields, where:</p>
<p>{</p>
<p> "type": "DRepVerificationKey_ed25519",</p>
<p> "description": "Delegate Representative Verification Key",</p>
<p> "cborHex": ""</p>
<p>}</p>
<p>{</p>
<p> "type": "DRepSigningKey_ed25519",</p>
<p> "description": "Delegate Representative VSigning Key",</p>
<p> "cborHex": ""</p>
<p>}</p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th rowspan="7">CLI09</th>
<th rowspan="7"><p>As a DRep</p>
<p>I want to generate a Drep Id</p>
<p>So that ada holder can use it to delegate their votes to me and my
voting record can be tracked</p></th>
<th><p><mark>The command is implemented as cardano-cli conway governance
drep id</mark></p>
<p><mark>and generates the blake2b-224 hash digest of the serialised
DRep credential (verification key)</mark></p></th>
<th><p>Typing cardano-cli conway governance drep id</p>
<p>with accepted input parameters generates a DRep ID, <mark>the
blake2b-224 hash digest of the serialised DRep credential (verification
key)</mark></p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The command accepts supplying the verification key with
either</mark></p>
<p><mark><br />
--drep-verification-key</mark></p>
<p><mark>–drep-verification-key-file options</mark></p></th>
<th><p>Using one of the flags is mandatory, the flags are mutually
exclusive and take a string and file respectively:</p>
<p><mark>--drep-verification-key &lt;- string</mark></p>
<p><mark>–drep-verification-key-file &lt;- file</mark></p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command supports the --out-file FILE option (optional) to
enable users to save the generated DRep ID to the specified
file.</mark></th>
<th>Given that the user wants to save the DrepId to a file, and
specifies a valid path and file name, then, using the –out-file flag
saves the drep id to a file on the specified location.<br />
<br />
If the specified path does not exist or is inaccessible the cli returns
an error message.<br />
<br />
If the –out-flag is not used the Drep ID is printed on stdout</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The command should support the an option to specify the
output format<br />
</mark></p>
<p><mark>Accepted output formats are "hex" and "bech32", where "bech32"
is the default format.</mark></p></th>
<th><p>Given that the optional --output-format flag is used, and
“bech32” is given as an argument, then the DRep Id is printed in bech32
format with the “drep” prefix.</p>
<p>Given that the optional --output-format flag is used, and the hex is
given as an argument, then the DRep Id is printed in hex format</p>
<p><mark>If the --output-format STRING option is <strong>not</strong>
specified, the DRep ID should be displayed in "bech32" format by
default.</mark></p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command supports an optional –out-file to save the Drep Id
to a file</mark></th>
<th><mark>If the --out-file FILE option is specified, the generated DRep
ID should be saved to the specified file, otherwise it is printed on
stdout</mark></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The feature is well-documented, providing clear usage
instructions for the cardano-cli conway governance drep id
command.</mark></th>
<th><p>Typing cardano-cli conway governance drep id --help</p>
<p>displays the command usage page</p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command handles errors gracefully and provides helpful
error messages when required options are missing or invalid inputs are
provided.</mark></th>
<th>If any required input parameter is missing or incorrect, the command
should raise an error indicating the missing or incorrect
parameter.</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="10">CLI10</th>
<th rowspan="10"><p>As a DRep</p>
<p>I want to generate a Drep registration certificate</p>
<p>So that I can submit it on a transaction and the ada holders can
delegate their votes to me.</p></th>
<th><p><mark>The command is implemented as</mark></p>
<p><mark>cardano-cli conway governance drep
registration-certificate</mark></p></th>
<th><p>Running</p>
<p><mark>cardano-cli conway governance drep
registration-certificate</mark> with accepted input parameters generates
a drep registration certificate.</p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The command requires the user to provide the amount
required for drep key deposit to comply with the conway cddl -&gt;
“reg_drep_cert”</mark></p></th>
<th>The flag --key-reg-deposit-amt is mandatory and takes the deposit
amount in lovelace as argument.</th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The command allows the user to provide the DRep credential
in the following ways:</mark></p>
<p>Drep verification key</p>
<p>Drep verification key file</p>
<p>Drep Id</p></th>
<th><p>The command presents the options to pass the Drep
credential:<br />
<br />
--drep-verification-key STRING</p>
<p>--drep-verification-key-file FILE</p>
<p>--drep-id STRING</p>
<p>Using one of these is mandatory but are mutually exclusive.</p>
<p>Failing to provide the right input results in a clear error message
that helps the user to identify the problem</p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command allows adding an optional anchor (url/hash) to
submit any drep metadata.</mark></th>
<th><p><mark>Given that the user wants to include an anchor with the
Dreps metadata, then the command requires both the url and the hash to
be provided. Only url or only hash is not allowed.<br />
<br />
--drep-metadata-url TEXT --drep-metadata-hash HASH</mark></p>
<p><mark><br />
</mark>Failing to provide the right input results in a clear error
message that helps the user to identify the problem</p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>When the --drep-metadata-url and
--drep-metadata-hash</mark></p>
<p><mark>are provided, the resulting certificate should include the url
and hash on the anchor position, otherwise the field is
null.</mark></p></th>
<th><p><mark>The anchor is included in the certificate on the last
position:</mark></p>
<p><mark>reg_drep_cert = (16, drep_credential, coin, anchor /
null)</mark></p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The --out-file FILE option is mandatory and used to specify
the file where the generated DRep registration certificate will be
saved.</mark></th>
<th><p>The flag <mark>--out-file</mark> is mandatory and takes the file
path and name as an argument.</p>
<p>Failure to provide the flag and its argument generates an
exception.</p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The command generates a registration certificate compliant
with the conway cddl</mark></p>
<p><mark><br />
</mark></p></th>
<th><mark>reg_drep_cert = (16, drep_credential, coin, anchor /
null)</mark></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The certificate should be on a text envelope format, similar
to what we have for stake pools registration certificates</mark></th>
<th><p>Given that the certificate is saved, then it is in a text
envelope format consisting of a json object with type, description and
cbor hex fields, where:</p>
<p><mark>{</mark></p>
<p> <mark>"type": "CertificateConway",</mark></p>
<p> <mark>"description": "DRep Registration Certificate",</mark></p>
<p> <mark>"cborHex": "00000000"</mark></p>
<p><mark>}</mark></p>
<p><mark></mark></p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The feature implementation should be well-documented,
providing clear usage instructions for the cardano-cli conway governance
drep registration-certificate command.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command should handle errors gracefully and provide
helpful error messages when required options are missing or invalid
inputs are provided.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="7">CLI11</th>
<th rowspan="7"><p>As a DRep</p>
<p>I want to generate a Drep retirement (unregistration) certificate</p>
<p>So that I can submit it on a transaction and can get my DRep deposit
back.</p></th>
<th><p><mark>The command allows the user to provide the DRep credentials
in the following ways:</mark></p>
<p><mark><strong>Using</strong> the --drep-verification-key STRING
option to specify the DRep verification key directly as a
string.</mark></p>
<p><mark><strong>Using</strong> the --drep-verification-key-file FILE
option to specify the file containing the DRep verification
key.</mark></p>
<p><mark><strong>Using</strong> the --drep-id STRING option to specify
the DRep ID directly as a string.</mark></p>
<p>cardano-cli conway governance drep retirement-certificate</p></th>
<th><p>Typing cardano-cli conway governance drep
retirement-certificate</p>
<p>with accepted input parameters will generate a DRep retirement
certificate.</p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command has the mandatory flag --deposit-amt to require
the user to provide the drep deposited amount that is to be
returned.<br />
<br />
Must match the deposit originally paid when registering as DRep but is
only checked when submitting the transaction.</mark></th>
<th><p>The flag <mark>--deposit-amt</mark> is mandatory and takes the
deposit amount in lovelace as an argument. The argument is a decimal,
providing any other type of input will result in an exception (no
implicit conversion)</p>
<p>Not providing the flag and its argument generates an
exception.</p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The --out-file FILE option should be mandatory and used to
specify the file where the generated DRep retirement certificate will be
saved</mark></th>
<th><p>The flag <mark>--out-file</mark> is mandatory and takes the file
path and name as an argument.</p>
<p>Failure to provide the flag and its argument generates an
exception.</p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The certificate should be on a text envelope format, similar
to what we have for stake pools deregistration certificates</mark></th>
<th><p>Given that the certificate is saved, then it is in a text
envelope format consisting of a json object with type, description and
cbor hex fields, where:</p>
<p><mark>{</mark></p>
<p> <mark>"type": "CertificateConway",</mark></p>
<p> <mark>"description": "DRep Retirement Certificate",</mark></p>
<p> <mark>"cborHex": "00000000"</mark></p>
<p><mark>}</mark></p>
<p><mark></mark></p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The output certificate complies with the conway cddl<br />
<br />
unreg_drep_cert = (17, drep_credential, coin)</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The feature implementation should be well-documented,
providing clear usage instructions</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command handles errors gracefully and provides helpful
error messages when required options are missing or invalid inputs are
provided.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th rowspan="4">CLI12</th>
<th rowspan="4"><p>As a Drep</p>
<p>I want to generate the hash of my DRep metadata</p>
<p>So that I can supply it when registering as DRep</p></th>
<th><p><mark>The command calculates the blake2b 256 hash of the file
supplied by the user.</mark></p>
<p>cardano-cli conway governance drep metadata-hash</p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command requires the --drep-metadata-file FILE option to
specify the file containing the DRep metadata.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command supports the --out-file FILE option (optional) to
enable users to save the calculated metadata hash to the specified file.
If the flag is not used, the hash is printed to stdout</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command handles errors gracefully and provides helpful
error messages when required options are missing or invalid inputs are
provided.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th rowspan="8">CLI13</th>
<th rowspan="8"><p>As an ada holder</p>
<p>I want to create a governance action that updates the
constitution</p>
<p>So that it can be submitted to the chain and be voted by the
governance bodies</p></th>
<th><p><mark>The command requires either --mainnet or --testnet-magic
NATURAL option to specify the target network for which the governance
action is generated</mark></p>
<p>cardano-cli conway governance action create-constitution</p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command requires the user to provide the the deposit
amount for submitting governance actions via the flag
<em>--governance-action-deposit</em></mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The command requires the user to provide the stake
credential that will receive the deposit return when the action is
enacted/expired. It accepts:<br />
</mark></p>
<p><mark>--stake-verification-key-file</mark></p>
<p><mark>--stake-verification-key</mark></p>
<p><mark>--stake-key-hash</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The command allows the user to provide the transaction id
and index of the previously enacted action of this type. These flags are
optional (but if one is used the other one must be used too) to support
the very first action of this type on the system which does not require
information about previously enacted actions. The flags are:</mark></p>
<p><mark>--governance-action-tx-id</mark></p>
<p><mark>--governance-action-index</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The command requires the user to provide an anchor (url /
hash) of the proposal. A document where the proposer exposes the
reasoning behind the proposed change.<br />
</mark></p>
<p><mark>--anchor-url</mark></p>
<p><mark>--anchor-data-hash</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The command requires the user to provide an anchor (url /
hash) of the new constitution.<br />
</mark></p>
<p><mark>--constitution-url</mark></p>
<p><mark>--constitution-hash</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command has the mandatory flag –out-file to specify the
file here the governance action (the proposal) will be
saved.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The generated governance action complies with the conway
cddl, where:<br />
</mark></p>
<p><mark>proposal_procedure =</mark></p>
<p> <mark>[ deposit : coin</mark></p>
<p> <mark>, reward_account</mark></p>
<p> <mark>, gov_action</mark></p>
<p> <mark>, anchor</mark></p>
<p> <mark>]</mark></p>
<p><mark>new_constitution = (5, gov_action_id / null,
constitution)</mark></p>
<p><mark>constitution =</mark></p>
<p> <mark>[ anchor</mark></p>
<p> <mark>, scripthash / null</mark></p>
<p> <mark>]</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th rowspan="10">CLI14</th>
<th rowspan="10"><p>As an ada holder</p>
<p>I want to create a governance action that updates the constitutional
committee</p>
<p>So that it can be submitted to the chain and be voted by the
governance bodies</p></th>
<th><mark>The command requires either --mainnet or --testnet-magic
NATURAL option to specify the target network for which the action is
generated</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command requires the user to provide the the deposit
amount for submitting governance actions via the flag
<em>--governance-action-deposit</em></mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The command requires the user to provide the stake
credential that will receive the deposit return when the action is
enacted/expired. It accepts:<br />
</mark></p>
<p><mark>--stake-verification-key-file</mark></p>
<p><mark>--stake-verification-key</mark></p>
<p><mark>--stake-key-hash</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The command requires the user to provide an anchor (url /
hash) of the proposal. A document where the proposer exposes the
reasoning behind the proposed change.<br />
</mark></p>
<p><mark>--anchor-url</mark></p>
<p><mark>--anchor-data-hash</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The command offers the option to remove many CC members, it
accepts:<br />
</mark></p>
<p><mark>--remove-cc-cold-verification-key-hash</mark></p>
<p><mark>--remove-cc-cold-verification-key</mark></p>
<p><mark>--remove-cc-cold-verification-key-file</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The command offers the option to add many CC members.<br />
</mark></p>
<p><mark>--add-cc-cold-verification-key</mark></p>
<p><mark>--add-cc-cold-verification-key-file</mark></p>
<p><mark>--add-cc-cold-verification-key-hash</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>When adding a new member, the command requires the user to
also provide a <strong>term</strong> for each new member using the flag
<strong>–epoch</strong></mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The command allows proposing a new quorum
threshold:</mark></p>
<blockquote>
<p><mark><strong>When</strong> adding members</mark></p>
<p><mark><strong>When</strong> removing members</mark></p>
<p><mark><strong>As</strong> standalone action (no adds or
removals)</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The command has the flag –out-file to specify the file
where the governance action (the proposal) will be
saved.</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The generated governance action complies with the conway
cddl, where:<br />
</mark></p>
<p><mark>proposal_procedure =</mark></p>
<p> <mark>[ deposit : coin</mark></p>
<p> <mark>, reward_account</mark></p>
<p> <mark>, gov_action</mark></p>
<p> <mark>, anchor</mark></p>
<p> <mark>]</mark></p>
<p><mark>update_committee = (4, gov_action_id / null,
set&lt;committee_cold_credential&gt;, { committee_cold_credential =&gt;
epoch }, unit_interval)</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th rowspan="8">CLI15</th>
<th rowspan="8"><p>As an ada holder</p>
<p>I want to create a governance action to withdraw funds from the
treasury</p>
<p>So that it can be submitted to the chain and be voted by the
governance bodies</p>
<p>cardano-cli conway governance action
create-treasury-withdrawal</p></th>
<th><mark>The command requires either --mainnet or --testnet-magic
NATURAL option to specify the target network for which the action is
generated</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command requires the user to provide the the deposit
amount for submitting governance actions via the flag
<em>--governance-action-deposit</em></mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The command requires the user to provide the stake
credential that will receive the deposit return when the action is
enacted/expired. It accepts:<br />
</mark></p>
<blockquote>
<p><mark>--stake-verification-key-file</mark></p>
<p><mark>--stake-verification-key</mark></p>
<p><mark>--stake-key-hash</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The command requires the user to provide an anchor (url /
hash) of the proposal. A document where the proposer exposes the
reasoning behind the proposed change.<br />
</mark></p>
<blockquote>
<p><mark>--anchor-url</mark></p>
<p><mark>--anchor-data-hash</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The command requires the user to provide the stake
credential that will receive the funds if the governance action is
ratified. It accepts:<br />
</mark></p>
<blockquote>
<p><mark>--stake-verification-key-file</mark></p>
<p><mark>--stake-verification-key</mark></p>
<p><mark>--stake-key-hash<br />
</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>Requires the user to provide the <strong>amount</strong> in
lovelace that will be transferred from the treasury to the stake
credential if the action is ratified.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command has the flag –out-file to specify the file where
the governance action (the proposal) will be saved.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The generated governance action complies with the conway
cddl, where:</mark></p>
<p><mark>proposal_procedure =</mark></p>
<p> <mark>[ deposit : coin</mark></p>
<p> <mark>, reward_account</mark></p>
<p> <mark>, gov_action</mark></p>
<p> <mark>, anchor</mark></p>
<p> <mark>]</mark></p>
<p><mark>treasury_withdrawals_action = (2, { reward_account =&gt; coin
})</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th rowspan="6">CLI16</th>
<th rowspan="6"><p>As an ada holder</p>
<p>I want to create an info governance action</p>
<p>So that it can be submitted to the chain and be voted by the
governance bodies</p>
<p>cardano-cli conway governance action create-info</p></th>
<th><mark>The command requires either --mainnet or --testnet-magic
NATURAL option to specify the target network for which the action is
generated.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command requires the user to provide the the deposit
amount for submitting governance actions via the mandatory flag
<em>--governance-action-deposit</em></mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The command requires the user to provide the stake
credential that will receive the deposit return when the action is
enacted/expired. It accepts:<br />
</mark></p>
<blockquote>
<p><mark>--stake-verification-key-file</mark></p>
<p><mark>--stake-verification-key</mark></p>
<p><mark>--stake-key-hash</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The command requires the user to provide an anchor (url /
hash) of the proposal. A document where the proposer exposes the
reasoning behind the proposed change.<br />
</mark></p>
<blockquote>
<p><mark>--anchor-url</mark></p>
<p><mark>--anchor-data-hash</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command has the flag –out-file to specify the file where
the governance action (the proposal) will be saved.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The generated governance action complies with the conway
cddl, where:</mark></p>
<p><mark>proposal_procedure =</mark></p>
<p> <mark>[ deposit : coin</mark></p>
<p> <mark>, reward_account</mark></p>
<p> <mark>, gov_action</mark></p>
<p> <mark>, anchor</mark></p>
<p> <mark>]</mark></p>
<p><mark>info_action = 6</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th rowspan="8">CLI17</th>
<th rowspan="8"><p>As an ada holder</p>
<p>I want to create a governance action to update protocol
parameters</p>
<p>So that it can be submitted to the chain and be voted by the
governance bodies</p>
<p>cardano-cli conway governance action
create-protocol-parameters-update</p></th>
<th><mark>The command requires either --mainnet or --testnet-magic
NATURAL option to specify the target network for which the DRep
registration certificate is generated.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command requires the user to provide the the deposit
amount for submitting governance actions via the mandatory flag
<em>--governance-action-deposit</em></mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The command requires the user to provide the stake
credential that will receive the deposit return when the action is
enacted/expired. It accepts:<br />
</mark></p>
<blockquote>
<p><mark>--stake-verification-key-file</mark></p>
<p><mark>--stake-verification-key</mark></p>
<p><mark>--stake-key-hash</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The command allows the user to provide the transaction id
and index of the previously enacted action of this type. These flags are
optional (but if one is used the other one must be used too) to support
the very first action of this type on the system which does not require
information about previously enacted actions. The flags are:</mark></p>
<blockquote>
<p><mark>--governance-action-tx-id</mark></p>
<p><mark>--governance-action-index</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The command requires the user to provide an anchor (url /
hash) of the proposal. A document where the proposer exposes the
reasoning behind the proposed change.<br />
</mark></p>
<blockquote>
<p><mark>--anchor-url</mark></p>
<p><mark>--anchor-data-hash</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The command includes dedicated flags to reference the
protocol parameter that the user is attempting to modify. The parameters
that can be included in this type of proposal are:<br />
</mark></p>
<p><mark>The <strong>network group</strong> consists of:</mark></p>
<blockquote>
<p><mark>maximum block body size (maxBBSize)</mark></p>
<p><mark>maximum transaction size (maxTxSize)</mark></p>
<p><mark>maximum block header size (maxBHSize)</mark></p>
<p><mark>maximum size of a serialized asset value
(maxValSize)</mark></p>
<p><mark>maximum script execution units in a single transaction
(maxTxExUnits)</mark></p>
<p><mark>maximum script execution units in a single block
(maxBlockExUnits)</mark></p>
<p><mark>maximum number of collateral inputs
(maxCollateralInputs)</mark></p>
</blockquote>
<p><mark>The <strong>economic group</strong> consists of:</mark></p>
<blockquote>
<p><mark>minimum fee coefficient (minFeeA)</mark></p>
<p><mark>minimum fee constant (minFeeB)</mark></p>
<p><mark>delegation key Lovelace deposit (keyDeposit)</mark></p>
<p><mark>pool registration Lovelace deposit (poolDeposit)</mark></p>
<p><mark>monetary expansion (rho)</mark></p>
<p><mark>treasury expansion (tau)</mark></p>
<p><mark>minimum fixed rewards cut for pools (minPoolCost)</mark></p>
<p><mark>minimum Lovelace deposit per byte of serialized UTxO
(coinsPerUTxOByte)</mark></p>
<p><mark>prices of Plutus execution units (prices)</mark></p>
</blockquote>
<p><mark>The <strong>technical group</strong> consists of:</mark></p>
<blockquote>
<p><mark>pool pledge influence (a0)</mark></p>
<p><mark>pool retirement maximum epoch (eMax)</mark></p>
<p><mark>desired number of pools (nOpt)</mark></p>
<p><mark>Plutus execution cost models (costModels)</mark></p>
<p><mark>proportion of collateral needed for scripts
(collateralPercentage)</mark></p>
</blockquote>
<p><mark>The <strong>governance group</strong> consists of all the new
protocol parameters that are introduced in this CIP:</mark></p>
<blockquote>
<p><mark>governance voting thresholds</mark></p>
<p><mark>dRepVotingThresholds</mark></p>
<p><mark>dvtCommitteeNoConfidence</mark></p>
<p><mark>dvtCommitteeNormal</mark></p>
<p><mark>dvtHardForkInitiation</mark></p>
<p><mark>dvtMotionNoConfidence</mark></p>
<p><mark>dvtPPEconomicGroup</mark></p>
<p><mark>dvtPPGovGroup</mark></p>
<p><mark>dvtPPNetworkGroup</mark></p>
<p><mark>dvtPPTechnicalGroup</mark></p>
<p><mark>dvtTreasuryWithdrawal</mark></p>
<p><mark>dvtUpdateToConstitution</mark></p>
<p><mark>poolVotingThresholds</mark></p>
<p><mark>pvtCommitteeNoConfidence</mark></p>
<p><mark>pvtCommitteeNormal</mark></p>
<p><mark>pvtHardForkInitiation</mark></p>
<p><mark>pvtMotionNoConfidence</mark></p>
<p><mark>governance action maximum lifetime in epochs
(govActionLifetime)</mark></p>
<p><mark>governance action deposit (govActionDeposit)</mark></p>
<p><mark>DRep deposit amount (drepDeposit)</mark></p>
<p><mark>DRep activity period in epochs (drepActivity)</mark></p>
<p><mark>minimal constitutional committee size (ccMinSize)</mark></p>
<p><mark>maximum term length (in epochs) for the constitutional
committee members (ccMaxTermLength)</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command has the flag –out-file to specify the file where
the governance action (the proposal) will be saved.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The generated governance action complies with the conway
cddl, where:</mark></p>
<p><mark>proposal_procedure =</mark></p>
<p> <mark>[ deposit : coin</mark></p>
<p> <mark>, reward_account</mark></p>
<p> <mark>, gov_action</mark></p>
<p> <mark>, anchor</mark></p>
<p> <mark>]</mark></p>
<p><mark>parameter_change_action = (0, gov_action_id / null,
protocol_param_update)</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th rowspan="7">CLI18</th>
<th rowspan="7"><p>As an ada holder</p>
<p>I want to create a no-confidence governance action</p>
<p>So that it can be submitted to the chain and be voted by the
governance bodies</p>
<p>cardano-cli conway governance action create-no-confidence</p></th>
<th><mark>The command requires either --mainnet or --testnet-magic
NATURAL option to specify the target network for which the action is
generated.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command requires the user to provide the the deposit
amount for submitting governance actions via the mandatory flag
<em>--governance-action-deposit</em></mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The command requires the user to provide the stake
credential that will receive the deposit return when the action is
enacted/expired. It accepts:<br />
</mark></p>
<blockquote>
<p><mark>--stake-verification-key-file</mark></p>
<p><mark>--stake-verification-key</mark></p>
<p><mark>--stake-key-hash</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The command allows the user to provide the transaction id
and index of the previously enacted action of this type. These flags are
optional (but if one is used the other one must be used too) to support
the very first action of this type on the system which does not require
information about previously enacted actions. The flags are:</mark></p>
<blockquote>
<p><mark>--governance-action-tx-id</mark></p>
<p><mark>--governance-action-index</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The command requires the user to provide an anchor (url /
hash) of the proposal. A document where the proposer exposes the
reasoning behind the proposed change.<br />
</mark></p>
<blockquote>
<p><mark>--anchor-url</mark></p>
<p><mark>--anchor-data-hash</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command has the flag –out-file to specify the file where
the governance action (the proposal) will be saved.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The generated governance action complies with the conway
cddl, where:</mark></p>
<p><mark>proposal_procedure =</mark></p>
<p> <mark>[ deposit : coin</mark></p>
<p> <mark>, reward_account</mark></p>
<p> <mark>, gov_action</mark></p>
<p> <mark>, anchor</mark></p>
<p> <mark>]</mark></p>
<p><mark>no_confidence = (3, gov_action_id / null)</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="8">CLI19</th>
<th rowspan="8"><p>As an ada holder</p>
<p>I want to create a governance action to initiate a hardfork</p>
<p>So that it can be submitted to the chain and be voted by the
governance bodies</p></th>
<th><mark>The command requires either --mainnet or --testnet-magic
NATURAL option to specify the target network for which the action is
generated.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command requires the user to provide the the deposit
amount for submitting governance actions via the mandatory flag
<em>--governance-action-deposit</em></mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The command requires the user to provide the stake
credential that will receive the deposit return when the action is
enacted/expired. It accepts:<br />
</mark></p>
<blockquote>
<p><mark>--stake-verification-key-file</mark></p>
<p><mark>--stake-verification-key</mark></p>
<p><mark>--stake-key-hash</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The command allows the user to provide the transaction id
and index of the previously enacted action of this type. These flags are
optional (but if one is used the other one must be used too) to support
the very first action of this type on the system which does not require
information about previously enacted actions. The flags are:</mark></p>
<blockquote>
<p><mark>--governance-action-tx-id</mark></p>
<p><mark>--governance-action-index</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The command requires the user to provide an anchor (url /
hash) of the proposal. A document where the proposer exposes the
reasoning behind the proposed change.<br />
</mark></p>
<blockquote>
<p><mark>--anchor-url</mark></p>
<p><mark>--anchor-data-hash</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command requires the user to input the <strong>new
protocol version number</strong></mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command has the flag –out-file to specify the file where
the governance action (the proposal) will be saved.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The generated governance action complies with the conway
cddl, where:</mark></p>
<p><mark>proposal_procedure =</mark></p>
<p> <mark>[ deposit : coin</mark></p>
<p> <mark>, reward_account</mark></p>
<p> <mark>, gov_action</mark></p>
<p> <mark>, anchor</mark></p>
<p> <mark>]</mark></p>
<p><mark>hard_fork_initiation_action = (1, gov_action_id / null,
[protocol_version])</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="4">CLI20</th>
<th rowspan="4"><p>As an ada holder</p>
<p>I want to inspect the contents of a governance action file</p>
<p>So that I can verify it is correct before submitting it in a
transaction</p>
<p>cardano-cli conway governance action view</p></th>
<th><mark>The command takes an action file as input</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>Gives an option to select the output format (json or
yaml)</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command has the flag –out-file to specify the file where
the output is saved, if it is not specified it is printed to
stdout</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The output shows the information of the proposal based on
the proposal procedures on a human readable format:<br />
<br />
proposal_procedure =</mark></p>
<p> <mark>[ deposit : coin</mark></p>
<p> <mark>, reward_account</mark></p>
<p> <mark>, gov_action</mark></p>
<p> <mark>, anchor</mark></p>
<p> <mark>]</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="6">CLI21</th>
<th rowspan="6"><p>As a Drep, SPO or CC member</p>
<p>I want to create a vote for a governance action</p>
<p>So that I can include it in a transaction and submit it to the
chain</p>
<p>cardano-cli conway governance vote create</p></th>
<th><p><mark>The command provides a way to vote</mark></p>
<blockquote>
<p><mark>yes,</mark></p>
<p><mark>no</mark></p>
<p><mark>abstain</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>Requires to specify the governance action ID and index that
the vote is about.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>Requires the user to provide DRep, SPO or CC
credentials</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The command allows the user to provide an optional anchor
(url / hash) if the user wishes to share the reasoning behind the
vote.<br />
</mark></p>
<blockquote>
<p><mark>--anchor-url</mark></p>
<p><mark>--anchor-data-hash</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command has the flag –out-file to specify the file where
the vote will be saved.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The generated vote complies with the conway cddl
where<br />
<br />
voting_procedures = { + voter =&gt; { + gov_action_id =&gt;
voting_procedure } }</mark></p>
<p><mark>voting_procedure =</mark></p>
<p> <mark>[ vote</mark></p>
<p> <mark>, anchor / null</mark></p>
<p> <mark>]</mark></p>
<p><mark>; no - 0</mark></p>
<p><mark>; yes - 1</mark></p>
<p><mark>; abstain - 2</mark></p>
<p><mark>vote = 0 .. 2</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="4">CLI22</th>
<th rowspan="4"><p>As a DRep, SPO or CC member</p>
<p>I want to inspect the contents of a vote file</p>
<p>So that I can verify it is correct before submitting it in a
transaction</p>
<p>cardano-cli conway governance vote view</p></th>
<th><mark>The command takes a vote file as an input</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>Gives an option to select the output format (json or
yaml)</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command has the flag –out-file to specify the file where
the output is saved, if it is not specified it is printed to
stdout</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The output shows the information of the proposal based on
the voting procedures in a human readable format (english):</mark></p>
<p><mark>voting_procedures = { + voter =&gt; { + gov_action_id =&gt;
voting_procedure } }</mark></p>
<p><mark>voting_procedure =</mark></p>
<p> <mark>[ vote</mark></p>
<p> <mark>, anchor / null</mark></p>
<p> <mark>]</mark></p>
<p><mark>; no - 0</mark></p>
<p><mark>; yes - 1</mark></p>
<p><mark>; abstain - 2</mark></p>
<p><mark>vote = 0 .. 2</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="2">CLI23</th>
<th rowspan="2"><p>As an ada holder</p>
<p>I want to build a transaction that includes a proposal (containing a
governance action)</p>
<p>So that I can later sign and submit to the chain</p>
<p>transaction build</p></th>
<th><mark>Transaction <strong>build</strong> has a new flag to supply a
proposal file as input for the transaction body</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>When constructing a transaction body that includes a
proposal, the resulting tx body conforms to the conway cddl so that
proposal procedures are recorded with the key 20<br />
</mark></p>
<p><mark>transaction_body =</mark></p>
<p> <mark>{ 0 : set&lt;transaction_input&gt; ; inputs</mark></p>
<p> <mark>, 1 : [* transaction_output]</mark></p>
<p> <mark>, 2 : coin ; fee</mark></p>
<p> <mark>, ? 3 : uint ; time to live</mark></p>
<p> <mark>, ? 4 : certificates</mark></p>
<p> <mark>, ? 5 : withdrawals</mark></p>
<p> <mark>, ? 7 : auxiliary_data_hash</mark></p>
<p> <mark>, ? 8 : uint ; validity interval start</mark></p>
<p> <mark>, ? 9 : mint</mark></p>
<p> <mark>, ? 11 : script_data_hash</mark></p>
<p> <mark>, ? 13 : nonempty_set&lt;transaction_input&gt; ; collateral
inputs</mark></p>
<p> <mark>, ? 14 : required_signers</mark></p>
<p> <mark>, ? 15 : network_id</mark></p>
<p> <mark>, ? 16 : transaction_output ; collateral return</mark></p>
<p> <mark>, ? 17 : coin ; total collateral</mark></p>
<p> <mark>, ? 18 : nonempty_set&lt;transaction_input&gt; ; reference
inputs</mark></p>
<p> <mark>, ? 19 : voting_procedures ; New; Voting procedures</mark></p>
<p> <strong><mark>, ? 20 : proposal_procedures ; New; Proposal
procedures</mark></strong></p>
<p> <mark>, ? 21 : coin ; New; current treasury value</mark></p>
<p> <mark>, ? 22 : positive_coin ; New; donation</mark></p>
<p> <mark>}</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="2">CLI24</th>
<th rowspan="2"><p>As a DRep, SPO or CC member</p>
<p>I want to build a transaction that includes my vote on a particular
governance action</p>
<p>So that I can later sign and submit to the chain</p>
<p>transaction build</p></th>
<th><mark>Transaction <strong>build</strong> has a new flag to supply a
vote file as input for the transaction body</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>When constructing a transaction body that includes a vote,
the resulting tx body conforms to the conway cddl so that voting
procedures are recorded with the key 19<br />
</mark></p>
<p><mark>transaction_body =</mark></p>
<p> <mark>{ 0 : set&lt;transaction_input&gt; ; inputs</mark></p>
<p> <mark>, 1 : [* transaction_output]</mark></p>
<p> <mark>, 2 : coin ; fee</mark></p>
<p> <mark>, ? 3 : uint ; time to live</mark></p>
<p> <mark>, ? 4 : certificates</mark></p>
<p> <mark>, ? 5 : withdrawals</mark></p>
<p> <mark>, ? 7 : auxiliary_data_hash</mark></p>
<p> <mark>, ? 8 : uint ; validity interval start</mark></p>
<p> <mark>, ? 9 : mint</mark></p>
<p> <mark>, ? 11 : script_data_hash</mark></p>
<p> <mark>, ? 13 : nonempty_set&lt;transaction_input&gt; ; collateral
inputs</mark></p>
<p> <mark>, ? 14 : required_signers</mark></p>
<p> <mark>, ? 15 : network_id</mark></p>
<p> <mark>, ? 16 : transaction_output ; collateral return</mark></p>
<p> <mark>, ? 17 : coin ; total collateral</mark></p>
<p> <mark>, ? 18 : nonempty_set&lt;transaction_input&gt; ; reference
inputs</mark></p>
<p> <strong><mark>, ? 19 : voting_procedures ; New; Voting
procedures</mark></strong></p>
<p> <mark>, ? 20 : proposal_procedures ; New; Proposal
procedures</mark></p>
<p> <mark>, ? 21 : coin ; New; current treasury value</mark></p>
<p> <mark>, ? 22 : positive_coin ; New; donation</mark></p>
<p> <mark>}</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="2">CLI25</th>
<th rowspan="2"><p>As an ada holder</p>
<p>I want to build a transaction that includes a proposal (containing a
governance action)</p>
<p>So that I can later sign and submit to the chain</p>
<p>transaction build-raw</p></th>
<th><mark>Transaction build-raw has a new flag to supply a proposal file
as input for the transaction body</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>When constructing a transaction body that includes a
proposal, the resulting tx body conforms to the conway cddl so that
proposal procedures are recorded with the key 20<br />
</mark></p>
<p><mark>transaction_body =</mark></p>
<p> <mark>{ 0 : set&lt;transaction_input&gt; ; inputs</mark></p>
<p> <mark>, 1 : [* transaction_output]</mark></p>
<p> <mark>, 2 : coin ; fee</mark></p>
<p> <mark>, ? 3 : uint ; time to live</mark></p>
<p> <mark>, ? 4 : certificates</mark></p>
<p> <mark>, ? 5 : withdrawals</mark></p>
<p> <mark>, ? 7 : auxiliary_data_hash</mark></p>
<p> <mark>, ? 8 : uint ; validity interval start</mark></p>
<p> <mark>, ? 9 : mint</mark></p>
<p> <mark>, ? 11 : script_data_hash</mark></p>
<p> <mark>, ? 13 : nonempty_set&lt;transaction_input&gt; ; collateral
inputs</mark></p>
<p> <mark>, ? 14 : required_signers</mark></p>
<p> <mark>, ? 15 : network_id</mark></p>
<p> <mark>, ? 16 : transaction_output ; collateral return</mark></p>
<p> <mark>, ? 17 : coin ; total collateral</mark></p>
<p> <mark>, ? 18 : nonempty_set&lt;transaction_input&gt; ; reference
inputs</mark></p>
<p> <mark>, ? 19 : voting_procedures ; New; Voting procedures</mark></p>
<p> <strong><mark>, ? 20 : proposal_procedures ; New; Proposal
procedures</mark></strong></p>
<p> <mark>, ? 21 : coin ; New; current treasury value</mark></p>
<p> <mark>, ? 22 : positive_coin ; New; donation</mark></p>
<p> <mark>}</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="2">CLI26</th>
<th rowspan="2"><p>As a DRep, SPO or CC member</p>
<p>I want to build a transaction that includes my vote on a particular
governance action</p>
<p>So that I can later sign and submit to the chain</p>
<p>transaction build-raw</p></th>
<th><mark>Transaction build-raw has a new flag to supply a vote file as
input for the transaction body</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>When constructing a transaction body that includes a vote,
the resulting tx body conforms to the conway cddl so that voting
procedures are recorded with the key 19<br />
</mark></p>
<p><mark>transaction_body =</mark></p>
<p> <mark>{ 0 : set&lt;transaction_input&gt; ; inputs</mark></p>
<p> <mark>, 1 : [* transaction_output]</mark></p>
<p> <mark>, 2 : coin ; fee</mark></p>
<p> <mark>, ? 3 : uint ; time to live</mark></p>
<p> <mark>, ? 4 : certificates</mark></p>
<p> <mark>, ? 5 : withdrawals</mark></p>
<p> <mark>, ? 7 : auxiliary_data_hash</mark></p>
<p> <mark>, ? 8 : uint ; validity interval start</mark></p>
<p> <mark>, ? 9 : mint</mark></p>
<p> <mark>, ? 11 : script_data_hash</mark></p>
<p> <mark>, ? 13 : nonempty_set&lt;transaction_input&gt; ; collateral
inputs</mark></p>
<p> <mark>, ? 14 : required_signers</mark></p>
<p> <mark>, ? 15 : network_id</mark></p>
<p> <mark>, ? 16 : transaction_output ; collateral return</mark></p>
<p> <mark>, ? 17 : coin ; total collateral</mark></p>
<p> <mark>, ? 18 : nonempty_set&lt;transaction_input&gt; ; reference
inputs</mark></p>
<p> <strong><mark>, ? 19 : voting_procedures ; New; Voting
procedures</mark></strong></p>
<p> <mark>, ? 20 : proposal_procedures ; New; Proposal
procedures</mark></p>
<p> <mark>, ? 21 : coin ; New; current treasury value</mark></p>
<p> <mark>, ? 22 : positive_coin ; New; donation</mark></p>
<p> <mark>}</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="6">CLI27</th>
<th rowspan="6"><p>As an ada holder</p>
<p>I want to create a conway cddl-compliant stake registration
certificate</p>
<p>stake-address</p></th>
<th><p><mark>Allows the user to provide credentials in any of the
following forms:</mark></p>
<blockquote>
<p><mark>Stake verification key</mark></p>
<p><mark>Stake verification key file</mark></p>
<p><mark>Stake address</mark></p>
<p><mark>Stake script file</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>Requires the user to provide the required key deposit in
lovelace</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command has the flag –out-file to specify the file where
the registration certificate will be saved.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command handles errors gracefully and provides helpful
error messages when required options are missing or invalid inputs are
provided.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The certificate should be saved on a text envelope
format:</mark></p>
<p><mark>{</mark></p>
<p> <mark>"type": "CertificateConway",</mark></p>
<p> <mark>"description": "Stake Address Registration
Certificate",</mark></p>
<p> <mark>"cborHex": ""</mark></p>
<p><mark>}</mark></p>
<p><mark></mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The resulting certificate conforms with the conway cddl,
where<br />
<br />
<strong>reg_cert = (7, stake_credential, coin)</strong></mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="6">CLI28</th>
<th rowspan="6"><p>As an ada holder</p>
<p>I want to create a conway cddl-compliant stake deregistration
certificate to get my deposit back</p>
<p>stake-address</p></th>
<th><p><mark>Allows the user to provide credentials in any of the
following forms:</mark></p>
<blockquote>
<p><mark>Stake verification key</mark></p>
<p><mark>Stake verification key file</mark></p>
<p><mark>Stake address</mark></p>
<p><mark>Stake script file</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>Requires the user to provide key deposit (in lovelace) that
was paid by the target stake credential when it registered</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command has the flag –out-file to specify the file where
the registration certificate will be saved.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command handles errors gracefully and provides helpful
error messages when required options are missing or invalid inputs are
provided.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The certificate should be saved on a text envelope
format:</mark></p>
<p><mark>{</mark></p>
<p> <mark>"type": "CertificateConway",</mark></p>
<p> <mark>"description": "Stake Address Deregistration
Certificate",</mark></p>
<p> <mark>"cborHex": ""</mark></p>
<p><mark>}</mark></p>
<p><mark></mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The resulting certificate conforms with the conway cddl,
where<br />
<br />
<strong>unreg_cert = (8, stake_credential, coin)</strong></mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="7">CLI29</th>
<th rowspan="7"><p>As an ada holder</p>
<p>I want to delegate my votes to a DRep (registered or default)</p>
<p>So that my stake is counted when the DRep vote.</p>
<p>Stake-address</p></th>
<th><p><mark>Allows the user to provide credentials in any of the
following forms:</mark></p>
<blockquote>
<p><mark>Stake verification key</mark></p>
<p><mark>Stake verification key file</mark></p>
<p><mark>Stake address</mark></p>
<p><mark>Stake script file</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>When delegating to a registered DRep, the user can provide
the target Drep with:<br />
</mark></p>
<blockquote>
<p><mark>DRep script hash</mark></p>
<p><mark>DRep verification key</mark></p>
<p><mark>DRep verification key file</mark></p>
<p><mark>DRep key hash (Drep ID)</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>When delegating to a default DRep the user can use a flag to
select either always-abstain or always-no-confidence, but not
both.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command has the flag –out-file to specify the file where
the vote delegation certificate will be saved.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command handles errors gracefully and provides helpful
error messages when required options are missing or invalid inputs are
provided.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The certificate should be saved on a text envelope
format:</mark></p>
<p><mark>{</mark></p>
<p> <mark>"type": "CertificateConway",</mark></p>
<p> <mark>"description": "Vote Delegation Certificate",</mark></p>
<p> <mark>"cborHex": ""</mark></p>
<p><mark>}</mark></p>
<p><mark></mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The resulting certificate conforms with the conway cddl,
where<br />
<br />
<strong>vote_deleg_cert = (9, stake_credential,
drep)</strong></mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th rowspan="8">CLI30</th>
<th rowspan="8"><p>As an ada holder</p>
<p>I want to delegate my stake to a stake pool AND my votes to a DRep
(registered or default) with a single certificate.</p>
<p>stake-address</p></th>
<th><p><mark>Allows the user to provide credentials in any of the
following forms:</mark></p>
<blockquote>
<p><mark>Stake verification key</mark></p>
<p><mark>Stake verification key file</mark></p>
<p><mark>Stake address</mark></p>
<p><mark>Stake script file</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The user can provide the target stake pool with:<br />
</mark></p>
<blockquote>
<p><mark>Stake pool cold verification key</mark></p>
<p><mark>Stake pool cold verification key file</mark></p>
<p><mark>Stake pool ID</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>Allows the user to provide the target DRep credential
with</mark></p>
<blockquote>
<p><mark>DRep script hash</mark></p>
<p><mark>DRep verification key</mark></p>
<p><mark>DRep verification key file</mark></p>
<p><mark>DRep key hash (Drep ID)</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>When delegating to a default DRep the user can use a flag to
select either always-abstain or always-no-confidence, but not
both.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command has the flag –out-file to specify the file where
the stake and vote delegation certificate will be saved.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command handles errors gracefully and provides helpful
error messages when required options are missing or invalid inputs are
provided.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The certificate should be saved on a text envelope
format:</mark></p>
<p><mark>{</mark></p>
<p> <mark>"type": "CertificateConway",</mark></p>
<p> <mark>"description": "Stake and Vote Delegation
Certificate",</mark></p>
<p> <mark>"cborHex": ""</mark></p>
<p><mark>}</mark></p>
<p><mark></mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The resulting certificate conforms with the conway cddl,
where<br />
<br />
<strong>stake_vote_deleg_cert = (10, stake_credential, pool_keyhash,
drep)</strong></mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th rowspan="5">CLI31</th>
<th rowspan="5"><p>As any persona</p>
<p>I want to query the nodes for the current</p>
<p>Governance state</p>
<p>So that I can inform my decisions</p></th>
<th><p><mark>The new command is implemented as cardano-cli conway query
gov-state</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command requires the user to specify the network id
(mainnet or testnet magic)</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command has the flag –out-file to specify the file where
the output will be saved.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>The output is a JSON showing, at least, the following
information:</mark></p>
<blockquote>
<p><mark><strong>Previous</strong> protocol parameters</mark></p>
<p><mark><strong>Current</strong> protocol parameters</mark></p>
<p><mark><strong>Last</strong> enacted governance actions IDs for
committee, constitution, hardfork initiation and parameter
updates</mark></p>
<p><mark><strong>Ratified</strong> governance actions that will be
enacted at next epoch transition</mark></p>
<p><mark><strong>Active</strong> governance actions proposals including
their type, stake address that collects the deposit, governance action
id, expiration, spo, drep and cc votes</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command handles errors gracefully and provides helpful
error messages when required options are missing or invalid inputs are
provided.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="8">CLI32</th>
<th rowspan="8"><p>As a CC member</p>
<p>I want to query the committee state</p>
<p>So that I can find my expiration term and whether my hot key
authorization certificate has been recorded on chain</p></th>
<th><mark>The command is implemented as cardano-cli conway query
committee-state</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>Requires the user to provide the network id</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>Supports a query for an specific CC credential<br />
</mark></p>
<blockquote>
<p><mark>CC cold verification key</mark></p>
<p><mark>CC cold verification key file</mark></p>
<p><mark>CC cold verification key hash</mark></p>
<p><mark>CC hot verification key</mark></p>
<p><mark>CC hot verification key file</mark></p>
<p><mark>CC hot verification key hash</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>When no CC key is specified, the command outputs information
for all committee members</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command allows filtering by active, expired and
unrecognized members (registered hot keys to an unknown cc cold
key)</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The output is a JSON showing, the following
information:</mark></p>
<blockquote>
<p><mark>Cold key hash</mark></p>
<p><mark>Hot credential status (Authorized/NotAuthorized)</mark></p>
<p><mark>When Authorized, shows the hot key hash</mark></p>
<p><mark>Status (Active, Expired, Unrecognized)</mark></p>
<p><mark>Expiration epoch</mark></p>
<p><mark>Current epoch (when you ran the query)</mark></p>
<p><mark>Quorum</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command has the flag –out-file to specify the file where
the output will be saved.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>The command handles errors gracefully and provides helpful
error messages when required options are missing or invalid inputs are
provided.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th rowspan="7">CLI33</th>
<th rowspan="7"><p>As an ada holder</p>
<p>I want to query the DRep state</p>
<p>So that …</p></th>
<th><mark>The command is implemented as cardano-cli conway query
drep-state</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>Requires the user to provide the network id</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>Supports a query for an specific DRep credential</mark></p>
<blockquote>
<p><mark>DRep verification key</mark></p>
<p><mark>DRep verification key file</mark></p>
<p><mark>DRep verification key hash (DRep ID)</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>If no Drep credential is specified it returns all
DReps</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command has the flag –out-file to specify the file where
the output will be saved.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The output is a JSON showing, the following
information:<br />
</mark></p>
<blockquote>
<p><mark>Drep Key hash</mark></p>
<p><mark>Anchor (Drep metadata)</mark></p>
<p><mark>Deposit</mark></p>
<p><mark>Expiry (from Drep activity)</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command handles errors gracefully and provides helpful
error messages when required options are missing or invalid inputs are
provided.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th rowspan="6">CLI34</th>
<th rowspan="6"><p>As an ada holder and DRep</p>
<p>I want to query the DRep stake distribution</p>
<p>So that I can find the weight (of the votes) of each DRep</p></th>
<th><mark>The command is implemented as cardano-cli conway query
drep-stake-distribution</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><p><mark>Supports a query for an specific DRep credential</mark></p>
<blockquote>
<p><mark>DRep verification key</mark></p>
<p><mark>DRep verification key file</mark></p>
<p><mark>DRep verification key hash (DRep ID)</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><mark>If no Drep credential is specified it returns all
DReps</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command has the flag –out-file to specify the file where
the output will be saved.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p><mark>The output is a JSON showing, the following
information:<br />
</mark></p>
<blockquote>
<p><mark>Drep Key hash</mark></p>
<p><mark>Stake delegated to this DRep</mark></p>
</blockquote></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><mark>The command handles errors gracefully and provides helpful
error messages when required options are missing or invalid inputs are
provided.</mark></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th>CLI35</th>
<th><p>As an ada holder,</p>
<p>I want to query my stake address information so that I can learn to
which pool and drep Im delegating to and the value in lovelace of my
deposits for delegating and for submitting governance actions.</p></th>
<th><mark>Expand the command query stake-address-info to return the drep
id of the DRep that the stake credential is delegated to and the value
of the existing deposits.</mark></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th></th>
<th>Script as a DRep</th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th colspan="6">Sidechain User Stories</th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th>CH.SID1</th>
<th>As a Sidechain, I wish to use BLS primitives to record settlement
operations on Cardano</th>
<th><p><a href="mailto:jon.rossie@iohk.io"><u>Jon
Rossie</u></a><mark>posted your ‘thread comments’ to
initiate</mark></p></th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th><strong>Detail Pending</strong></th>
<th>Sidechain</th>
<th></th>
</tr>
<tr class="header">
<th>CH.SID2</th>
<th>Sidechain will use BLS for tokenomics, in particular to support
multi-sig certificates about Sidechain activity that can be verified by
Plutus contracts</th>
<th>Detail Pending</th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th><strong>Detail Pending</strong></th>
<th>Sidechain</th>
<th></th>
</tr>
<tr class="odd">
<th colspan="6">Plutus Component Level User Stories</th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th>CIP-85</th>
<th>As a DApp developer I would like to use sums-of-products instead of
Scott-encoding in my Plutus scripts to get better performance</th>
<th>Sums-of-products is available to use in Plutus V3 scripts and is the
default way of encoding data types in Plutus Tx.</th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th>Plutus</th>
<th></th>
</tr>
<tr class="odd">
<th>CIP-101</th>
<th>User stories for Keccak256 primitive</th>
<th>Detail Pending</th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th>Plutus</th>
<th></th>
</tr>
<tr class="header">
<th></th>
<th>As a DApp developer I want to use the Blake2b-224 hashing function
to compute PubKeyHash onchain</th>
<th>The Blake2b-224 is available to use in Plutus V3 after the HF</th>
<th><strong>Detail Pending</strong></th>
<th></th>
<th></th>
<th>Plutus</th>
<th></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

# Revision & Approval

<table style="width:84%;">
<colgroup>
<col style="width: 9%" />
<col style="width: 18%" />
<col style="width: 7%" />
<col style="width: 26%" />
<col style="width: 20%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Name</strong></th>
<th><strong>Position</strong></th>
<th><strong>Role</strong></th>
<th><strong>Comments</strong></th>
<th><strong>Status</strong></th>
</tr>
<tr class="odd">
<th><a href="mailto:mike.ward@iohk.io"><u>Mike Ward</u></a></th>
<th>Chief Product Officer</th>
<th>Approver</th>
<th></th>
<th>Under Review</th>
</tr>
<tr class="header">
<th><a href="mailto:michael.madoff@iohk.io"><u>Michael
Madoff</u></a></th>
<th>Product Manager - Voltaire</th>
<th>Approver</th>
<th></th>
<th>Under Review</th>
</tr>
<tr class="odd">
<th><a href="mailto:samuel.leathers@iohk.io"><u>Samuel
Leathers</u></a></th>
<th>Product Manager - Core Tech</th>
<th>Approver</th>
<th></th>
<th>Under Review</th>
</tr>
<tr class="header">
<th><a href="mailto:dorin.solomon@iohk.io"><u>Dorin Solomon</u></a></th>
<th>Quality Chapter Director</th>
<th>Approver</th>
<th></th>
<th></th>
</tr>
<tr class="odd">
<th><a href="mailto:carlos.lopezdelara@iohk.io"><u>Carlos Lopez de
Lara</u></a></th>
<th>Product Owner - Core Tech</th>
<th>Reviewer</th>
<th></th>
<th>Under Review</th>
</tr>
<tr class="header">
<th><a href="mailto:kevin.hammond@iohk.io"><u>Kevin Hammond</u></a></th>
<th>Head of Technology - Core Tech</th>
<th>Approver</th>
<th></th>
<th>Under Review</th>
</tr>
<tr class="odd">
<th><a href="mailto:lorenzo.bruno@iohk.io"><u>Lorenzo Bruno</u></a></th>
<th>Product Design Lead - Voltaire Governance Tools</th>
<th>Reviewer</th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><a href="mailto:thomas.upfield@iohk.io"><u>Thomas
Upfield</u></a></th>
<th>Product Owner - Voltaire</th>
<th>Reviewer</th>
<th></th>
<th>Under Review</th>
</tr>
<tr class="odd">
<th><a href="mailto:gerard.moroney@iohk.io"><u>Gerard
Moroney</u></a></th>
<th>COO</th>
<th>Reviewer</th>
<th></th>
<th>Under Review</th>
</tr>
<tr class="header">
<th><a href="mailto:omer.husain@iohk.io"><u>Omer Husain</u></a></th>
<th>Product Manager - Plutus</th>
<th>Reviewer</th>
<th>Confirm Smart Contracts User Stories</th>
<th>To Be Added</th>
</tr>
<tr class="odd">
<th><a href="mailto:billy.mullins@iohk.io"><u>Billy Mullins</u></a></th>
<th>VP Cardano</th>
<th>Reviewer</th>
<th>Confirm All User Stories</th>
<th>Under Review</th>
</tr>
<tr class="header">
<th><a href="mailto:dominik.zajkowski@iohk.io"><u>Dominik
Zajkowski</u></a></th>
<th>Sidechains Architect</th>
<th>Reviewer</th>
<th>Confirm Sidechains User Stories</th>
<th>Detail Pending</th>
</tr>
<tr class="odd">
<th><a href="mailto:arnaud.bailly@iohk.io"><u>Arnaud Bailly</u></a></th>
<th>Hydra Architect</th>
<th>Reviewer</th>
<th>Confirm Hydra User Stories</th>
<th></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

# 
