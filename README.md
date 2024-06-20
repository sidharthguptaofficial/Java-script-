# NFT Collection Manager

A JavaScript project for creating, storing, and displaying a collection of NFTs (Non-Fungible Tokens) with detailed metadata.

## Features

- *Create NFTs*: Generate NFTs with specific metadata including title, color, style, and medium.
- *Store NFTs*: Maintain a collection of NFTs in an array.
- *Display NFTs*: List all NFTs in the collection with their metadata.
- *Total Count*: Retrieve and display the total number of NFTs created.

## Getting Started

### Prerequisites

- A modern web browser or Node.js environment.

### Installation

No installation is required. Copy the provided code into your JavaScript environment and execute it.

## Usage

1. *Creating NFTs*:
   Use the createNFT function to create new NFTs with specific metadata.
   javascript
   createNFT("Aurora", "Green", "Impressionism", "Acrylic");
   createNFT("Blaze", "Red", "Abstract", "Digital");
   

2. *Displaying NFTs*:
   Use the displayNFTs function to print the details of all NFTs in the collection.
   javascript
   displayNFTs();
   

3. *Getting Total Number of NFTs*:
   Use the getNFTCount function to print the total number of NFTs created.
   javascript
   getNFTCount();
   

## Code Explanation

### Variables and Class Definition

javascript
let nftCollection = [];
let totalNFTs = 0;


- nftCollection: An array to store all NFT objects.
- totalNFTs: A counter to keep track of the total number of NFTs created.

### Class Definition

javascript
class DigitalArt {
    constructor(title, hue, genre, medium) {
        this.title = title;
        this.hue = hue;
        this.genre = genre;
        this.medium = medium;
    }
}


- DigitalArt: A class to define the structure of an NFT with properties title, hue, genre, and medium.

### Functions

#### Create an NFT

javascript
function createNFT(title, hue, genre, medium) {
    const nft = new DigitalArt(title, hue, genre, medium);
    nftCollection.push(nft);
    totalNFTs++;
}


- createNFT: This function creates a new DigitalArt object (NFT) with the provided metadata and adds it to the nftCollection. It also increments the totalNFTs counter.

#### Display All NFTs

javascript
function displayNFTs() {
    console.log("Displaying the list of all NFTs:\n");
    nftCollection.forEach((nft, index) => {
        console.log(`NFT ${index + 1}: Title - ${nft.title}, Color - ${nft.hue}, Style - ${nft.genre}, Medium - ${nft.medium}\n`);
    });
}


- displayNFTs: This function loops through the nftCollection array and prints the details of each NFT, including its index in the collection.

#### Get Total Number of NFTs

javascript
function getNFTCount() {
    console.log("Total number of NFTs created:");
    console.log(totalNFTs);
}


- getNFTCount: This function prints the total number of NFTs created by displaying the value of totalNFTs.

### Example Usage

javascript
createNFT("Aurora", "Green", "Impressionism", "Acrylic");
createNFT("Blaze", "Red", "Abstract", "Digital");

displayNFTs();
getNFTCount();


- *createNFT*: Creates two NFTs with the specified properties.
- *displayNFTs*: Prints the metadata of all created NFTs.
- *getNFTCount*: Prints the total number of NFTs created.

## License

This contract is licensed under the MIT License. SPDX-License-Identifier: MIT.
---

Feel free to adjust any section to better suit your project's needs.

## author name 
Sidharth gupta 
## uid 
21bcs11398
