# pixelheads
A library that makes it easy to retrieve skins and faces of minecraft players based on their uuid.

## Usage
1. Run `npm install pixelheads`
2. Use one of the functions to retrieve the skin or the face as a base64-encoded string.
   ```ts
     import pixelheads from "pixelheads";
     
     // Returns the entire skin of the player as a base64-encoded string. 
     const playerSkin = pixelheads.getSkinAsBase64("uuid"); 
   
     // Returns the face of the player as a base64-encoded string.
     const playerFace = pixelheads.getFaceAsBase64("uuid"); 
   ```
3. Use one of the return values, e.g. in an `img`-tag:
   ```
   <img src="'data:image/png;base64,' + playerFace" alt="face of player"></img>
   ```

## Building
Prerequisites:
- Git
- Node.js and npm
- TypeScript installed globally (`npm install -g typescript`)

Run the following commands:
```sh
git clone https://github.com/jojomatik/pixelheads
cd pixelheads
npm install
```

To build, run the following commands:
```sh
tsc
```

To pack the project as a tarball, run the following commands:
```sh
npm pack
```

## Licensing
This project is licensed under the MIT License (MIT). See also [`LICENSE`](LICENSE).
