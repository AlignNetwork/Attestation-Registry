<h2 align="center">Attestation Registry (⌐🔷_🔷) </h2>
<br />
<p align="center">

<br/>
<a href="https://twitter.com/align_network">Twitter</a> | 
<a href="https://warpcast.com/~/channel/align">Warpcast</a>
  
</p>

This repository acts as a registry for attestation providers to make other users aware of their custom attestation setups.
<br/><br />

### Example

Say the Pudgy Penguins wants to hand out a badge for each user that attends their event at ETH Denver. 

The psudeocode attestation would look like this:

```
{
  "Attester": "Pudgy Penguins",
  "Claim": "This holder attended an ETH Denver event"
  "Claim Proof": "Link to lu.ma or similar event app"
}
```

Pudgy's now create a PR in this repo and allow everyone to use this attestation claim type provided they follow the rules.

The rules would be as follows:

1. Recipient must have attended the event.
2. The event must have been a registered side event at ETH denver.
3. Claim Proof must be provided in the form of a link to attendees and event page.

Now anyone can use this claim type to attest that someone went to their event and provided they stake a certain amount of ETH for the attestations. If challenged, this ETH could potentially be slashed if it was found the attester lied.

Finally, at the end of ETH Denver, a DeFi protocol can query this specific Claim Type and get a verified list of participants and airdrop an NFT to each participant.
