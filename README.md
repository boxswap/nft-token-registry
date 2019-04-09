# NFT Token Registry
A collection of data on NFT tokens that give users information such as supported standards and 
alternative ways to get token metadata. 

## Submission Proccess
1. Fork this repository.<br/>
2. Add Submission<br/>

Sample Submission: <br/>

```json
	"0xf87e31492faf9a91b02ee0deaad50d51d56d5d4d": {
		"name": "Decentraland",
		"symbol": "LAND",
		"type": "erc721",
		"tokenMetadataUrl": "https://api.decentraland.org/v1/parcels/{x}/{y}",
		"tokenMetadataUrlFromContract": "tokenMetadata(uint256 tokenID)"
	}
```
With placeholder identifiers: 

```json
	{contract_address}: {
		"name": {token_name},
		"symbol": {token_symbol},
		"type": {token_type},
		"tokenMetadataUrl": {token_metadata_url},
		"tokenMetadataUrlFromContract": {token_metadata_url_abi_method}
	}
```

## Token types
**ERC721** implements all base methods of the ERC721 standard<br/>
**ERC721a** doesn't implement approvalForAll methods<br/>
**ERC721b**  doesn't implement transferFrom methods<br/>

## Recommended standards
**ERC721** https://github.com/OpenZeppelin/openzeppelin-solidity/blob/master/contracts/token/ERC721/IERC721Full.sol<br/>

## Issues
If you'd like to make suggestions, ask for help, or file a bug: Make a new issue!
