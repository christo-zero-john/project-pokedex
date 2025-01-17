I want to create a device like pokedex in the pokemon anime. It works like this:

- First I have a website with data of all pokemons.
- I will supply rfid cards with a unique identifier in the market.
- I also have a mobile app which works like the app of smartwatches.
- The pokedex can be connected with smartphones using bluetooth.
- When this rfid is readed by my pokedex, it then send the unique id that is stored in the rfid to my mobile app. The mobile app then display the data of that pokemon on the app.
- Also the user can create account in my website via the mobile app.
- Once the unique identifier is recieved by the mobile app, it registers that unique id with that user account.
- Every pokemon in the database has numerous unique identifiers. These identifiers are one time use only. Once the user scans that pokemon using the pokedex, the app then marks that identifier as used.
- After registering the unique identifier with the user account, I will then write the pokemon-id of the pokemon which is related to that unique identifier in the rfid to the pokedex via the mobile app.
- The pokedex will then store the pokemon-id related to that unique identifier.
- This counts as the user catching a pokemon.
- Every unique identifier has a random power value assosciated with it. If the user reads the unique identifier of same pokemon from other cards, the power value of his/her pokemon is added.
- If the power value of a pokemon reaches 25, the star of the pokemon is incremented by 1. If the pokemon becomes 5 star, it can be evolved.
- For every generation of pokemon, the stars needed to be evolved is 4 + generation of pokemon.
- If the pokemon is basic pokemon, then its generation is 1.
- If the pokemon has evolved n times, its generation will be n+1.

- If the rfid card with that same unique identifier is read by the some other pokedex, the user will get an eror that tells him, the card is already registered with someone elses account.

## The Pokedex and RFID

- The pokedex is a device that can be connected to mobile device via bluetooth.
- It has a storage size of 4GB.
- It stores user-id, client-id (which is some identifier used to identify the mobile device), an array of pokemon-id's, (which is the ID of pokemon's that the user owns), and the unique identifier of the rfid card from which the pokemon is collected or catched by the user.
- It also stores the data of the pokemon that the user has in their collection.
- A single pokedex could store a maximum of 200 pokemon's.
- It also has an RGB light, some buttons, speaker etc...
- It exactly looks and works like the pokedex in pokemon anime except that, it only stores data of the pokemon that the user owns.
- When connected to the smartphone via bluetooth, it could identify any pokemon that is stored in any RFID.
- When the user queries over the pokemon via the pokedex, the pokedex will speak out name, description etc... of the pokemon through the speaker. Ath the same time, the rgb light plays some interesting light patterns just like the pokedex in pokemon anime.
- Querying pokemon happens when:
  - User queries through the pokemon they owns.
  - When User reads the pokemon using an rfid, (the data is fetched from the smartphone and outputs through the pokedex).

## Hardwares Required

- RFID card
- RF Reader.
- Micro controller Unit.(ESP32, ESP8266, Arduino)
- Storage.(SSD, HDD, Micro SD)
- Bluetooth module.(HC-05, HC-06, BTHome)

## Softwares Required

- Mobile App
- Website
- Database 
