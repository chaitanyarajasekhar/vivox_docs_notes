### Channels & Users
- Channels & Users are identified by uniform resource identifiers(URIs)
- Assigned by the game

### Utilizing vivox capabilities 
- Map player ID's with viox user URI's, typically *games use the player ID as a protion of the vivox URI*.
- Maping game audio/tesxt enabled objects to vivox channel URIs. typically *Games use the game object identifier as a portion of the vivox channel URI*.
- When user logins also log in the vivox system, enable access tokens on the vivox instance serving the game.
- make game server to deliver vivox access tokens to game clients (JSON web tokens wit one time permission)

#### Access Tokens uses
- login users
- add to specific channel
- kick from channel
- muting user

### Client Basics 
- initialize client sdk
- setup message polling - check for new messages
- messaging types - event,response 
- Request and Responses 
- connector obj - after it is created the game can login to vivox
- Login
- uninitialize


### Client SDK voice and text basics 
- Joining a channnel - game maps audio element to the channel 
- Direct text and voice basics 

### Text to speech 

### Client SDK presence basics 
- buddy 

### Client SDK advanced topics 
- Logs
- Enabling selection of audio device 
- Setting audio leves 
- Mute Users
- Kick
- Echo
- Multi Channel 
- Character Encoding 

## Core Integration 
### Basics 
- COre elemnts: vivox network, server & client api, sip uri
- Game Server elements: account & channel management, access token management & third party call controll
- Game client elements: login management, channel management, user interface controls , error handling

### Planning and organization 
- Login management: unquie Id, user logins must be approved way ahead of game implementation, after approval of the login the game 
assigns a user Id to cleint which is used along with the access token 
- channel management 
- Game server integration: after choosing the login schemes, plan to use them in server
- Authorization: tokens to secure loginin, join channels, perform certain acctions 
- UI integration 

### Implementation 
- build a bassic application 

### Testing
- Some test: UI elements, UI functions, loggin checkpoints
- Feature Checkpoints:

### Additional developer information 
- Login
- Channels: Persistent/ semi-persistant, echo channels
- Access tokens:
- UI integration

## Core API Refernce 
### Modules
- Initialize 
- Sending and receiving messages
- Memory management 
- Login in/out
- Group voice text communication 
- Audio Devices 
- Diagnostics
- Mobile
- COnsoles 
### Data Structures 

### Access Tokens guide
- Only used once and can expire with time
- Token format: VAT - vivox access token - Json web token
- Payload: The payload is a base64url-encoded JSON object that contains the claims asserted by the token
- Signature: The signature is the base64url-encoded HMAC of the first two parts
- Supported values for vivox action (vxa claim)

### Example Tokens
- Generating tokens on the client 
- Generating tokens on the server


### Server to Server APIs
- Game ServersHTTP POST calls -> vivox system -> returns data in XML
- Game server to provide access tokens when client needs it 


### Text Chat developer guide
