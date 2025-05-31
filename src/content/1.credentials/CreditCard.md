# CreditCard

```json
{
    "@context": ["https://www.w3.org/2018/credentials/v1"],
    "type": ["VerifiableCredential", "CreditCard"],
    "credentialSubject": {
        "cardNumber": "1234-5678-9011-1234",
        "ownerName": "JOHN DOE",
        "expiryDate": "01/2030",
        "CVV": 123,
        "id": "identity#bankId"
    },
    "id": "identity#BankId#3add94f4-28ec-42a1-8704-4e4aa51006b4",
    "issued": "2025-06-01T00:00:00Z",
    "issuer": {
        "id": "did:key:z6MkrHKzgsahxBLyNAbLQyB1pcWNYC9GmywiWPgkrvntAZcj",
        "image": {
            "id": "https://images.squarespace-cdn.com/content/v1/609c0ddf94bcc0278a7cbdb4/1660296169313-K159K9WX8J8PPJE005HV/Walt+Bot_Logo.png?format=100w",
            "type": "Image"
        },
        "name": "CH Authority",
        "type": "Profile",
        "url": "https://images.squarespace-cdn.com/content/v1/609c0ddf94bcc0278a7cbdb4/1660296169313-K159K9WX8J8PPJE005HV/Walt+Bot_Logo.png?format=100w"
    },
    "validFrom": "2025-06-01T00:00:00Z",
    "issuanceDate": "2025-06-01T00:00:00Z"
}
```

## Manifest

```json
{
    "claims": {
        "Card Number": "$.credentialSubject.cardNumber",
        "Owner Name": "$.credentialSubject.ownerName"
    }
}
```

## Mapping example

```json
{
    "id": "<uuid>",
    "issuer": {
        "id": "<issuerDid>"
    },
    "credentialSubject": {
        "id": "<subjectDid>"
    },
    "issuanceDate": "<timestamp>"
}
```