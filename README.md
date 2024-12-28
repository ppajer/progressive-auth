# Progressive Auth

> *Monorepo of libraries that implement a full-stack, modular &amp; plugin-based solution to progressively adding modern auth methods to web &amp; hybrid apps.*


### Auth methods supported:

- Password
- OAuth
- Web3
- WebAuthn

### Tech stacks:

- React
- NodeJS
- NextJS
- PHP/Laravel

### Contents

1. Interface Definitions
2. Database Schemas
3. Frontend Components
4. API Libraries
5. User Classes & Factory
6. Plugins



## 1. Interface Definitions [In progress]
```
LoginRequest {
  method: "password" | "web3" | "oauth" | "webauthn"
  payload: PasswordAuthPayload | Web3AuthPayload | OAuthPayload | WebAuthnPayload
  csrf: string
}

PasswordAuthPayload {
  username: string
  password: string
}

Web3AuthPayload {
  username: string
  signature: string
}

OAuthPayload {
  token: string
}

WebAuthnPayload {
  passkey: string
}
```
