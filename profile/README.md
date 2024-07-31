> [!CAUTION]
> The ``arcuno.co`` domain is no longer supported as of the date ``31.07.2024 DD/MM/YYYY``

---

[<img alt="Static Badge" src="https://img.shields.io/badge/Twitter-%2369ADCF?style=for-the-badge&logo=X">](https://twitter.com/@ArcunoNetwork)  [<img alt="Static Badge" src="https://img.shields.io/badge/Discord-69ADCF?style=for-the-badge&logo=Discord">](https://discord.gg/q7bPDwrDkx)

# Arcuno Network
**Join us on the Arcuno Network! We offer many fun game modes, with our own coming soon. Experience our tight-knit community and cross-compatibility from versions ``1.7.x`` to ``1.8.x`` Don't miss out on fun events — give us a try today!**

### Game Modes
**At Arcuno Network we offer many game modes such as ``NODEBUFF`` ``CLASSIC`` ``SUMO`` ``BOXING`` ``GAPPLE`` and many more!**

### Social Impact
**At Arcuno Network we try to support OSS software while our infrastructere is closed-source our other projects are distributed under a ``MIT`` license**

### Documents
- [Copyright](https://arcuno.co/docs/Copyright.pdf)
- [TermsOfService](https://arcuno.co/docs/TermsOfService.pdf)
- [PrivacyPolicy](https://arcuno.co/docs/PrivacyPolicy.pdf)

## Arcuno API 

> [!WARNING]  
> **Your API usage may be RateLimited depending on the current server load**

**Current API status can be seen [here](https://status.arcuno.co)**

## Usage
   * Send a ``GET`` request to ``https://arcuno.net/api/v1/API_PATH``
     
## Endpoints

### 1. Get Global Statistics
**URL:** `/stats/global`

**Method:** `GET`

**Query Parameters:**
- `max` (optional): Maximum number of players to return. Defaults to 10.
- `sort` (optional): Sorting criterion. Defaults to `highestGlobalWinStreak`.

**Response:**
- `200 OK`: Returns an array of sorted global statistics.
- `500 Internal Server Error`: Returns an error message if there is a server error.

### 2. Get Category Statistics
**URL:** `/stats/:category`

**Method:** `GET`

**URL Parameters:**
- `category`: The category for which statistics are requested.

**Query Parameters:**
- `sort` (optional): Sorting criterion. Defaults to `highestStreak`.
- `max` (optional): Maximum number of entries to return. Defaults to 10.

**Response:**
- `200 OK`: Returns an array of sorted statistics for the specified category.
- `500 Internal Server Error`: Returns an error message if there is a server error.

### 3. Get Player Data
**URL:** `/stats/player/:username`

**Method:** `GET`

**URL Parameters:**
- `username`: The username of the player for which data is requested.

**Response:**
- `200 OK`: Returns the data of the specified player.
- `404 Not Found`: Returns an error message if the player is not found.
- `500 Internal Server Error`: Returns an error message if there is a server error.

### 4. Get Documentation Data for Player
**URL:** `/playerlist/player/:username`

**Method:** `GET`

**URL Parameters:**
- `username`: The username of the player for which documentation data is requested.

**Response:**
- `200 OK`: Returns the documentation data of the specified player.
- `404 Not Found`: Returns an error message if the player is not found.
- `500 Internal Server Error`: Returns an error message if there is a server error.

### 5. Get Player List
**URL:** `/playerlist/list`

**Method:** `GET`

**Query Parameters:**
- `details` (optional): If `true`, returns detailed information about each player. Defaults to `false`.

**Response:**
- `200 OK`: Returns a list of players.
- `500 Internal Server Error`: Returns an error message if there is a server error.

--- 


**© 2024 Arcuno Network**
