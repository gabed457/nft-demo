#NFT Making and Minting

To enter the Truffle console run

```truffle develop```

Create the NFT accessible variable in the console

```const helloNFT = await HelloNFTContract.deployed();```

Example NFT JSON:

```json
{
	"name": "Hello, NFTs!",
	"description": "Animated GIF that displays the text 'Hello, NFTs!' in 3 colors: Red, Green, and Blue.",
	"image": "http://adilmoujahid.com/images/intro-nfts-solidity/hello-nfts-rgb.gif"
}
```

Mint the above JSON into an NFT

``` helloNFT.mintNFT("http://adilmoujahid.com/files/hello-nfts-rgb.json")```

Mint NFT JSON & assign owner

```helloNFT.mintNFT("http://adilmoujahid.com/files/hello-nfts-rgb.json",{from:accounts[3]})```

Get address of NFT owner

``` helloNFT.ownerOf(1)```

Get NFT Token URI

```helloNFT.tokenURI(1)```
