# MyAPI Documentation

## Overview
This document describes the API endpoints for **MyAPI** (version v3), which provides functionality for retrieving user account details and managing betting operations. The API uses the OpenAPI 3.0.1 specification and requires Bearer token authentication (JWT format) for all requests.

---

## Authentication
All endpoints require a Bearer token for authentication. Include the token in the `Authorization` header as follows:

```
Authorization: Bearer <your-token>
```

---

## Endpoints

### 1. Get User Account Details
**GET** `/api/penalty/operator/{operatorId}/game/{gameId}/accounts`

#### Summary
Retrieves user details for a specified user token.

#### Parameters
- **operatorId** (path, required, string): Operator ID from the route.
- **gameId** (path, required, string): Game ID from the route.

#### Responses
- **200 OK**: User information retrieved successfully.
  - **Content Types**: `text/plain`, `application/json`, `text/json`
  - **Schema**: `UserInfoDto`
    ```json
    {
      "username": "string",
      "balance": number
    }
    ```
  - **Examples**:
    - **Demo User**: `{"username":"demo-user","balance":1250.75}`
    - **Zero Balance**: `{"username":"empty-wallet","balance":0}`
    - **High Roller**: `{"username":"big-player","balance":99999.99}`
- **400 Bad Request**: Operator or Game ID mismatch.
- **401 Unauthorized**: Unauthorized access.
- **404 Not Found**: Account not found.

---

### 2. Get Betting History
**GET** `/api/penalty/operator/{operatorId}/game/{gameId}/bets`

#### Summary
Retrieves betting history information for a user.

#### Parameters
- **operatorId** (path, required, string): Operator ID from the route.
- **gameId** (path, required, string): Game ID from the route.

#### Responses
- **200 OK**: Bet history information retrieved successfully.
  - **Content Types**: `text/plain`, `application/json`, `text/json`
  - **Schema**: `BetHistoryResponse`
    ```json
    {
      "bets": [
        {
          "id": "string",
          "type": integer,
          "amount": integer,
          "number": integer,
          "isWin": boolean,
          "createdAt": integer
        }
      ]
    }
    ```
  - **Example**:
    - **Basic History**: `{"bets":[{"id":"79d5ccdac7b53f9a7fd858a0f3eb0c25","type":1,"amount":100,"number":7,"isWin":true,"createdAt":1714500000}]}`
- **400 Bad Request**: Operator or Game ID mismatch.
- **401 Unauthorized**: Unauthorized access.
- **404 Not Found**: Bet history information not found.

---

### 3. Place a Bet
**POST** `/api/penalty/operator/{operatorId}/game/{gameId}/bets`

#### Summary
Places a bet for a user.

#### Parameters
- **operatorId** (path, required, string): Operator ID from the route.
- **gameId** (path, required, string): Game ID from the route.

#### Request Body
- **Content Types**: `application/json`, `text/json`, `application/*+json`
- **Schema**: `PlaceBetCommand`
  ```json
  {
    "bets": [
      {
        "amount": integer,
        "number": integer,
        "type": integer
      }
    ],
    "clientTime": integer
  }
  ```
- **Description**:
  - `bets`: List of bets to be placed.
  - `clientTime`: Time when the bet was initiated on the client side (UTC, integer).

#### Responses
- **200 OK**: Bet placed successfully.
  - **Content Types**: `text/plain`, `application/json`, `text/json`
  - **Schema**: `PlaceBetResponse`
    ```json
    {
      "playerResult": [
        {
          "id": "string",
          "type": integer,
          "winAmount": integer,
          "value": integer
        }
      ],
      "gameResult": {
        "type": integer,
        "value": integer,
        "isWin": boolean
      },
      "winAmount": integer,
      "balanceAfter": number
    }
    ```
  - **Examples**:
    - **Win Example**: `{"playerResult":[{"id":null,"type":1,"winAmount":200,"value":null}],"gameResult":{"type":1,"value":9,"isWin":false},"winAmount":200,"balanceAfter":1450.75}`
    - **Lose Example**: `{"playerResult":[{"id":null,"type":1,"winAmount":0,"value":null}],"gameResult":{"type":1,"value":8,"isWin":false},"winAmount":0,"balanceAfter":1240.5}`
- **400 Bad Request**: Operator or Game ID mismatch.
- **401 Unauthorized**: Unauthorized access.
- **403 Forbidden**: Forbidden action.

---

## Schemas

### UserInfoDto
```json
{
  "username": "string",
  "balance": number
}
```

### BetHistoryResponse
```json
{
  "bets": [
    {
      "id": "string",
      "type": integer,
      "amount": integer,
      "number": integer,
      "isWin": boolean,
      "createdAt": integer
    }
  ]
}
```

### PlaceBetCommand
```json
{
  "bets": [
    {
      "amount": integer,
      "number": integer,
      "type": integer
    }
  ],
  "clientTime": integer
}
```

### PlaceBetResponse
```json
{
  "playerResult": [
    {
      "id": "string",
      "type": integer,
      "winAmount": integer,
      "value": integer
    }
  ],
  "gameResult": {
    "type": integer,
    "value": integer,
    "isWin": boolean
  },
  "winAmount": integer,
  "balanceAfter": number
}
```

### BetTypeEnum
Enum of valid bet types: `[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]`

### ProblemDetails
```json
{
  "type": "string",
  "title": "string",
  "status": integer,
  "detail": "string",
  "instance": "string"
}
```

---

## Security
The API uses a Bearer token (JWT format) for authentication. Ensure the token is valid and included in all requests.

For more details, contact the API provider or refer to the official documentation at [https://x.ai/api](https://x.ai/api).
