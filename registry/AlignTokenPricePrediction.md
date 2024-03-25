<h2 align="center">Align Token Price Prediction </h2><br />

<h4>Creator/Attestor: Align Network</h4>
This Attestation signifies a price prediction on a crypto asset. It allows users or bots to make a prediction about the future price of a token as an attestation. The price prediction must follow the rules and disputes must be handled according to the resolution section. 
<br/><br />

Psudeocode:

```
{
  "Attester": "Align Network",
  "Claim": "I think the price of BTC_USD will be $46,000 on April 24,2024 (unix:1714058782), leeway +/- 1%.",
  "Claim Proof": "<ipfs_link>"
}
```

### Claim Rules:
The claim must mention:
  1. The base asset (enumerator)
  2. The quote asset (denominator)
  3. Specific Price
  4. Leeway (+/- margin of error for prediction)
  5. The time, preferable as a Unix [timestamp](https://www.unixtimestamp.com/) to settle the attestation

### Resolution

After the Time to settle has passed, anyone can resolve this claim by either marking the claim as false or true. Since this claim is realtivly easy to check with NLP and a connection to a price website such as [coingecko](https://www.coingecko.com/) a bot is inplace to verify the claims. For the Stage 1 period, we are not allowing user disputes on this attestation.
