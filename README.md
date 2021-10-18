# Introduction to Smart Contract 
#### The short description of all custom methods on Smart Contract
*Compiler Version* - *v0.8.0*
*ERC Version* - *721*

## Required Packages for Compilation
 - @openzeppelin/contracts
 - chai
 - chai-as-promised
 - web3
 - truffle
 - ganache-cli

## Writing Methods

**AddToAllowList** -
    ***required parameter - user address***

> The method is used to add the users to the white list

**mint** - ***required parameters:***
   - payableAmount(ether)
   - to(address)
   - count of minting items(**NUMBER**)

> This method is called when starting the sale of the NFTs

**preSaleMint** -
    ***required parameters:***
   - payableAmount(ether)
   - count of minting items(**NUMBER**)

> This method is called when starting the presale of the NFTs. You do not need the user address because you have it  when add them on the whiteList by using the ***addToAllowList*** method

**removeFromAllowList** -
    ***required parameter - user address***

> The method is used to remove the users from the white list

**removeFromAllowList** -
    ***required parameter - user address***

> The method is used to remove the users from the white list

**reserveNft** -
    ***required parameter - count***

> The method is used to reserve the nfts which will be redirected to the owner's account

**setActive** -
    ***required parameter - true/false***

> The method is used to turn on/off minting

**setAllowListMaxMint** -
    ***required parameter - NUMBER***

> The method is used to limit the minting count per user on presale stage 

**setBaseURI** -
    ***required parameter - string***

> need to fill

**setIsAllowListActive** -
    ***required parameter - true/false***

> The method is used to turn on/off presale start

**setMaxReserve** -
    ***required parameter - NUMBER***

> The method is used to limit the owner's maximum reservation count

**setMaximumAllowedTokens** -
    ***required parameter - NUMBER***

> The method is used to limit the maximum nfts count per purchase

**setPrice** -
    ***required parameter - NUMBER***

> The method is used to define the price for NFT

**setReserveAtATime** -
    ***required parameter - NUMBER***

> need to fill

**transferFrom** -
    ***required parameters:***
    - from address
   - to address
   - tokenID ( nft id )

> Method is used for giveaways or for transferring specific items between accounts

**withdraw** -    **We sure you know for what it is ;) **

## Reading Methods

**MAX_MINTSUPPLY** -
> The maximum allowed mint count.

**allowListClaimedBy** -
    ***required parameter - owner address***

> The method is return the list of adresses on the white list.

**allowListMaxMint** -
> Maximum minting count on presale phase

**balanceOf** -
    ***required parameter - owner address***

> The method is used to check the balance of the owner

**mintPrice** -
> returns number
> The Price of the NFT


**checkIfOnAllowList** -
    ***required parameter - user address***
> returns string
> The method is used to check address is on the white list.


**getContractOwner** -
> returns string
> Returns contract owner address

**getMaximumAllowedTokens** -
> returns *maximumAllowedTokensPerPurchase*

**getPrice** -
> returns number
> returns price

**getReserveAtATime** -
> returns number
> The count of reserved tokens per each click

**getTotalSupply** -
> returns number
> The total number of minted NFTs

**isActive** -
> return true/false
> describes whether the sale starts or not

**isAllowListActive** -
> return true/false
> describes whether the presale starts or not


**maximumAllowedTokensPerPurchase** -
> returns number
> The count of maximum allowed NFTs per purchase

**name** -
> returns string
> returns Name of the Collection

**owner** -
> returns string
> returns the Collection owner address

**ownerOf** -
***required parameter - tokenID(NUMBER)***
> returns string
> returns the specific NFTs owner address
