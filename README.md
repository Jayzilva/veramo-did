### DID

`veramo did create`

`did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910`

```
{
  "didDocumentMetadata": {},
  "didResolutionMetadata": {
    "contentType": "application/did+ld+json"
  },
  "didDocument": {
    "@context": [
      "https://www.w3.org/ns/did/v1",
      "https://w3id.org/security/suites/secp256k1recovery-2020/v2"
    ],
    "id": "did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910",
    "verificationMethod": [
      {
        "id": "did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910#controller",
        "type": "EcdsaSecp256k1RecoveryMethod2020",
        "controller": "did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910",
        "blockchainAccountId": "eip155:1:0xcaf3C37a127793a4934a7e2831FfEDD9E83Cc8b1"
      },
      {
        "id": "did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910#controllerKey",
        "type": "EcdsaSecp256k1VerificationKey2019",
        "controller": "did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910",
        "publicKeyHex": "0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910"
      }
    ],
    "authentication": [
      "did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910#controller",
      "did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910#controllerKey"
    ],
    "assertionMethod": [
      "did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910#controller",
      "did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910#controllerKey"
    ]
  }
}
```

---

`veramo credential create`

- jwt

```
{
  credentialSubject: {
    'Sample Name': 'Alice',
    id: 'did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910'
  },
  issuer: {
    id: 'did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910'
  },
  type: [ 'VerifiableCredential', 'Verifible' ],
  credentialStatus: {
    type: 'EthrStatusRegistry2019',
    id: 'goerli:0x97fd27892cdcD035dAe1fe71235c636044B59348'
  },
  '@context': [
    'https://www.w3.org/2018/credentials/v1',
    'https://veramo.io/contexts/profile/v1'
  ],
  issuanceDate: '2023-11-16T15:38:26.000Z',
  proof: {
    type: 'JwtProof2020',
    jwt: 'eyJhbGciOiJFUzI1NksiLCJ0eXAiOiJKV1QifQ.eyJ2YyI6eyJAY29udGV4dCI6WyJodHRwczovL3d3dy53My5vcmcvMjAxOC9jcmVkZW50aWFscy92MSIsImh0dHBzOi8vdmVyYW1vLmlvL2NvbnRleHRzL3Byb2ZpbGUvdjEiXSwidHlwZSI6WyJWZXJpZmlhYmxlQ3JlZGVudGlhbCIsIlZlcmlmaWJsZSJdLCJjcmVkZW50aWFsU3ViamVjdCI6eyJTYW1wbGUgTmFtZSI6IkFsaWNlIn0sImNyZWRlbnRpYWxTdGF0dXMiOnsidHlwZSI6IkV0aHJTdGF0dXNSZWdpc3RyeTIwMTkiLCJpZCI6ImdvZXJsaToweDk3ZmQyNzg5MmNkY0QwMzVkQWUxZmU3MTIzNWM2MzYwNDRCNTkzNDgifX0sInN1YiI6ImRpZDpldGhyOjB4MDMyODkzOWMzZGM1YWYyOWZlNTJmZWEyYWI5NzAxOWQyNTZhNmZmZDE3ZTdiYmMwOTQwNWUxNTQ2NmYyNTNjOTEwIiwibmJmIjoxNzAwMTQ5MTA2LCJpc3MiOiJkaWQ6ZXRocjoweDAzMjg5MzljM2RjNWFmMjlmZTUyZmVhMmFiOTcwMTlkMjU2YTZmZmQxN2U3YmJjMDk0MDVlMTU0NjZmMjUzYzkxMCJ9.lIO12bObmQy06nc0MPv3AQs96uScJEgBxpSYS1_5wog-WH4D_LeXHtuf-hUNXUe096FXArNmPYdIhgBHVozQwQ'
  }
```

- lds

```
{
  issuer: {
    id: 'did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910'
  },
  '@context': [
    'https://www.w3.org/2018/credentials/v1',
    'https://w3id.org/security/suites/secp256k1recovery-2020/v2'
  ],
  type: [ 'VerifiableCredential', 'Profile' ],
  issuanceDate: '2023-11-16T16:00:54.790Z',
  credentialSubject: {
    id: 'did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910',
    name: 'Alice'
  },
  credentialStatus: {
    type: 'EthrStatusRegistry2019',
    id: 'goerli:0x97fd27892cdcD035dAe1fe71235c636044B59348'
  },
  proof: {
    type: 'EcdsaSecp256k1RecoverySignature2020',
    created: '2023-11-16T16:01:03Z',
    verificationMethod: 'did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910#controller',
    proofPurpose: 'assertionMethod',
    jws: 'eyJhbGciOiJFUzI1NkstUiIsImI2NCI6ZmFsc2UsImNyaXQiOlsiYjY0Il19..vUIGKNRbTHwkXVPzw-GS455DjDBxgT3e_X-TrPvH6I1Rg_Ea-IzJ4OTJw9VCuvMizJRL39P6I0el_KywiGxvHwE'
  }
}
```

- EthereumEip712Signature2021

```
{
  issuer: {
    id: 'did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910'
  },
  '@context': [
    'https://www.w3.org/2018/credentials/v1',
    'https://veramo.io/contexts/profile/v1'
  ],
  type: [ 'VerifiableCredential', 'Profile' ],
  issuanceDate: '2023-11-16T16:20:05.204Z',
  credentialSubject: {
    id: 'did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910',
    name: 'Alice'
  },
  credentialStatus: {
    type: 'EthrStatusRegistry2019',
    id: 'goerli:0x97fd27892cdcD035dAe1fe71235c636044B59348'
  },
  proof: {
    verificationMethod: 'did:ethr:0x0328939c3dc5af29fe52fea2ab97019d256a6ffd17e7bbc09405e15466f253c910#controller',
    created: '2023-11-16T16:20:05.204Z',
    proofPurpose: 'assertionMethod',
    type: 'EthereumEip712Signature2021',
    proofValue: '0x63bc34a57c7f8dfc76972c7714014ad85107efbc8c2eee2195e5806fc301ff0a1f44f61d785ebb972e84f30090ae5e95f318e6cb05ec5b7ebd7c3e3b874702ef1c',
    eip712: {
      domain: { chainId: 1, name: 'VerifiableCredential', version: '1' },
      types: {
        EIP712Domain: [
          { name: 'name', type: 'string' },
          { name: 'version', type: 'string' },
          { name: 'chainId', type: 'uint256' }
        ],
        CredentialStatus: [
          { name: 'id', type: 'string' },
          { name: 'type', type: 'string' }
        ],
        CredentialSubject: [
          { name: 'id', type: 'string' },
          { name: 'name', type: 'string' }
        ],
        Issuer: [ { name: 'id', type: 'string' } ],
        Proof: [
          { name: 'created', type: 'string' },
          { name: 'proofPurpose', type: 'string' },
          { name: 'type', type: 'string' },
          { name: 'verificationMethod', type: 'string' }
        ],
        VerifiableCredential: [
          { name: '@context', type: 'string[]' },
          { name: 'credentialStatus', type: 'CredentialStatus' },
          { name: 'credentialSubject', type: 'CredentialSubject' },
          { name: 'issuanceDate', type: 'string' },
          { name: 'proof', type: 'Proof' },
          { name: 'type', type: 'string[]' }
        ]
      },
      primaryType: 'VerifiableCredential'
    }
  }
}
```
