# DesignatedVerifier

```json
{
    "@context": ["https://www.w3.org/2018/credentials/v1", "ndid:context:DesignatedVerifier"],
    "id": "0x5ff0713ae0e29ca52a7799370a82534fdf0f25d6e82ae5645e827f0ac34eaf4b",
    "type": ["VerifiableCredential", "DesignatedVerifier"],
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
    "issuanceDate": "2025-06-01T07:21:13.591Z",
    "credentialSubject": {
        "verifierID": "123456",
        "allowedCredentialTypes": ["CreditCard"]
    },
    "credentialStatus": {
        "id": "0x2ef196ba560d7d72f13d80f405841bc84cec229b70a0a05557c5388d215bb224",
        "type": "NDIDCredentialStatus2021"
    },
    "credentialSchema": {
        "id": "ndid:schema:walletHolder",
        "type": "JsonSchemaValidator2018"
    }
}
```

## Manifest

```json
{
    "claims": {
        "Verifier ID": "$.credentialSubject.verifierID"
    }
}
```

## Mapping example

```json
{
    "id": "<uuid>",
    "issuer": {
        "id" : "<issuerDid>"
    },
    "credentialSubject": {
        "verifierID": "<subjectDid>"
    },
    "issuanceDate": "<timestamp>",
    "expiryDate": "<timestamp>"
}
```