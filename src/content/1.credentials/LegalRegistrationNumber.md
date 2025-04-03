# LegalRegistrationNumber

```json
{
  "@context": [
    "https://www.w3.org/2018/credentials/v1",
    "https://w3id.org/security/suites/jws-2020/v1"
  ],
  "type": [
    "VerifiableCredential",
    "LegalRegistrationNumber"
  ],
  "id": "https://www.delta-dao.com/.well-known/2210_gx_registrationnumber.json",
  "issuer": "did:web:www.delta-dao.com:notary:v1",
  "issuanceDate": "2025-02-23T16:42:16.058Z",
  "credentialSubject": {
    "@context": "https://registry.lab.gaia-x.eu/development/api/trusted-shape-registry/v1/shapes/jsonld/trustframework#",
    "type": "gx:legalRegistrationNumber",
    "id": "https://www.delta-dao.com/.well-known/2210_gx_registrationnumber.json",
    "gx:leiCode": "391200FJBNU0YW987L26",
    "gx:leiCode-countryCode": "DE"
  },
  "evidence": [
    {
      "gx:evidenceURL": "https://api.gleif.org/api/v1/lei-records/",
      "gx:executionDate": "2025-02-23T16:42:16.058Z",
      "gx:evidenceOf": "gx:leiCode"
    }
  ]
}
```

## Manifest

```json
{
    "claims": {
        "Legal Registration Number": "$.credentialSubject.id",
        "LEI Code": "$.credentialSubject['gx:leiCode']",
        "LEI Country Code": "$.credentialSubject['gx:leiCode-countryCode']"
    }
}
```

## Mapping example

```json
{
  "id": "<uuid>",
  "issuer": "<issuerDid>",
  "credentialSubject": {
    "id": "<subjectDid>"
  },
  "issuanceDate": "<timestamp>",
  "expirationDate": "<timestamp-in:365d>"
}
```