 Sūrya's Description Report

 Files Description Table


|  File Name  |  SHA-1 Hash  |
|-------------|--------------|
| /Users/kunanonjarat/Developer/Bitkub-Smart-Contract/TMG-NFT/TMG-NFT.sol | 82d734141ee76c6a7a592b17994194f669f0a96c |


 Contracts Description Table


|  Contract  |         Type        |       Bases      |                  |                 |
|:----------:|:-------------------:|:----------------:|:----------------:|:---------------:|
|     └      |  **Function Name**  |  **Visibility**  |  **Mutability**  |  **Modifiers**  |
||||||
| **IKAP165** | Interface |  |||
| └ | supportsInterface | External ❗️ |   |NO❗️ |
||||||
| **KAP165** | Implementation | IKAP165 |||
| └ | supportsInterface | Public ❗️ |   |NO❗️ |
||||||
| **IAdminProjectRouter** | Interface |  |||
| └ | isSuperAdmin | External ❗️ |   |NO❗️ |
| └ | isAdmin | External ❗️ |   |NO❗️ |
||||||
| **Authorization** | Implementation |  |||
| └ | <Constructor> | Public ❗️ | 🛑  |NO❗️ |
| └ | setAdmin | External ❗️ | 🛑  | onlySuperAdmin |
| └ | setTransferRouter | External ❗️ | 🛑  | onlySuperAdmin |
||||||
| **Committee** | Implementation |  |||
| └ | setCommittee | External ❗️ | 🛑  | onlyCommittee |
||||||
| **IKYCBitkubChain** | Interface |  |||
| └ | kycsLevel | External ❗️ |   |NO❗️ |
||||||
| **KYCHandler** | Implementation |  |||
| └ | _activateOnlyKycAddress | Internal 🔒 | 🛑  | |
| └ | _setKYC | Internal 🔒 | 🛑  | |
| └ | _setAcceptedKycLevel | Internal 🔒 | 🛑  | |
||||||
| **Pauseable** | Implementation |  |||
| └ | <Constructor> | Public ❗️ | 🛑  |NO❗️ |
| └ | _pause | Internal 🔒 | 🛑  | whenNotPaused |
| └ | _unpause | Internal 🔒 | 🛑  | whenPaused |
||||||
| **IKAP721** | Interface | IKAP165 |||
| └ | balanceOf | External ❗️ |   |NO❗️ |
| └ | ownerOf | External ❗️ |   |NO❗️ |
| └ | safeTransferFrom | External ❗️ | 🛑  |NO❗️ |
| └ | transferFrom | External ❗️ | 🛑  |NO❗️ |
| └ | adminTransfer | External ❗️ | 🛑  |NO❗️ |
| └ | internalTransfer | External ❗️ | 🛑  |NO❗️ |
| └ | externalTransfer | External ❗️ | 🛑  |NO❗️ |
| └ | approve | External ❗️ | 🛑  |NO❗️ |
| └ | getApproved | External ❗️ |   |NO❗️ |
| └ | setApprovalForAll | External ❗️ | 🛑  |NO❗️ |
| └ | isApprovedForAll | External ❗️ |   |NO❗️ |
| └ | safeTransferFrom | External ❗️ | 🛑  |NO❗️ |
||||||
| **IKAP721Receiver** | Interface |  |||
| └ | onKAP721Received | External ❗️ | 🛑  |NO❗️ |
||||||
| **IKAP721Metadata** | Interface |  |||
| └ | name | External ❗️ |   |NO❗️ |
| └ | symbol | External ❗️ |   |NO❗️ |
| └ | tokenURI | External ❗️ |   |NO❗️ |
| └ | kapURI | External ❗️ |   |NO❗️ |
||||||
| **IKAP721Enumerable** | Interface |  |||
| └ | totalSupply | External ❗️ |   |NO❗️ |
| └ | tokenOfOwnerByIndex | External ❗️ |   |NO❗️ |
| └ | tokenByIndex | External ❗️ |   |NO❗️ |
||||||
| **Address** | Library |  |||
| └ | isContract | Internal 🔒 |   | |
||||||
| **EnumerableSetUint** | Library |  |||
| └ | add | Internal 🔒 | 🛑  | |
| └ | remove | Internal 🔒 | 🛑  | |
| └ | contains | Internal 🔒 |   | |
| └ | length | Internal 🔒 |   | |
| └ | at | Internal 🔒 |   | |
| └ | getAll | Internal 🔒 |   | |
| └ | get | Internal 🔒 |   | |
||||||
| **EnumerableMap** | Library |  |||
| └ | _set | Private 🔐 | 🛑  | |
| └ | _remove | Private 🔐 | 🛑  | |
| └ | _contains | Private 🔐 |   | |
| └ | _length | Private 🔐 |   | |
| └ | _at | Private 🔐 |   | |
| └ | _tryGet | Private 🔐 |   | |
| └ | _get | Private 🔐 |   | |
| └ | _get | Private 🔐 |   | |
| └ | set | Internal 🔒 | 🛑  | |
| └ | remove | Internal 🔒 | 🛑  | |
| └ | contains | Internal 🔒 |   | |
| └ | length | Internal 🔒 |   | |
| └ | at | Internal 🔒 |   | |
| └ | tryGet | Internal 🔒 |   | |
| └ | get | Internal 🔒 |   | |
| └ | get | Internal 🔒 |   | |
||||||
| **Strings** | Library |  |||
| └ | toString | Internal 🔒 |   | |
||||||
| **KAP721** | Implementation | IKAP721, IKAP721Metadata, IKAP721Enumerable, KAP165, Authorization, Committee, KYCHandler, Pauseable |||
| └ | <Constructor> | Public ❗️ | 🛑  | Authorization |
| └ | activateOnlyKycAddress | Public ❗️ | 🛑  | onlyCommittee |
| └ | setKYC | Public ❗️ | 🛑  | onlyCommittee |
| └ | setAcceptedKycLevel | Public ❗️ | 🛑  | onlyCommittee |
| └ | pause | Public ❗️ | 🛑  | onlyCommittee |
| └ | unpause | Public ❗️ | 🛑  | onlyCommittee |
| └ | supportsInterface | Public ❗️ |   |NO❗️ |
| └ | balanceOf | Public ❗️ |   |NO❗️ |
| └ | ownerOf | Public ❗️ |   |NO❗️ |
| └ | tokenURI | Public ❗️ |   |NO❗️ |
| └ | kapURI | Public ❗️ |   |NO❗️ |
| └ | totalSupply | Public ❗️ |   |NO❗️ |
| └ | tokenOfOwnerByIndex | Public ❗️ |   |NO❗️ |
| └ | tokenByIndex | Public ❗️ |   |NO❗️ |
| └ | approve | Public ❗️ | 🛑  |NO❗️ |
| └ | getApproved | Public ❗️ |   |NO❗️ |
| └ | setApprovalForAll | Public ❗️ | 🛑  |NO❗️ |
| └ | isApprovedForAll | Public ❗️ |   |NO❗️ |
| └ | transferFrom | Public ❗️ | 🛑  |NO❗️ |
| └ | adminTransfer | External ❗️ | 🛑  | onlyCommittee |
| └ | internalTransfer | External ❗️ | 🛑  | onlySuperAdminOrTransferRouter |
| └ | externalTransfer | External ❗️ | 🛑  | onlySuperAdminOrTransferRouter |
| └ | safeTransferFrom | Public ❗️ | 🛑  |NO❗️ |
| └ | safeTransferFrom | Public ❗️ | 🛑  |NO❗️ |
| └ | _safeTransfer | Internal 🔒 | 🛑  | |
| └ | _exists | Internal 🔒 |   | |
| └ | _isApprovedOrOwner | Internal 🔒 |   | |
| └ | _safeMint | Internal 🔒 | 🛑  | |
| └ | _safeMint | Internal 🔒 | 🛑  | |
| └ | _mint | Internal 🔒 | 🛑  | whenNotPaused |
| └ | _burn | Internal 🔒 | 🛑  | whenNotPaused |
| └ | _transfer | Internal 🔒 | 🛑  | whenNotPaused |
| └ | _approve | Internal 🔒 | 🛑  | |
| └ | _setTypeURI | Internal 🔒 | 🛑  | |
| └ | _setBaseURI | Internal 🔒 | 🛑  | |
| └ | _setKapURI | Internal 🔒 | 🛑  | |
| └ | _setBaseKapURI | Internal 🔒 | 🛑  | |
| └ | _checkOnKAP721Received | Private 🔐 | 🛑  | |
| └ | _beforeTokenTransfer | Internal 🔒 | 🛑  | |
||||||
| **ITheMallNft** | Interface |  |||
| └ | mintInfo | External ❗️ |   |NO❗️ |
| └ | exists | External ❗️ |   |NO❗️ |
| └ | tokenOfOwnerByPage | External ❗️ |   |NO❗️ |
| └ | tokenOfOwnerAll | External ❗️ |   |NO❗️ |
| └ | setTypeURI | External ❗️ | 🛑  |NO❗️ |
| └ | setBaseURI | External ❗️ | 🛑  |NO❗️ |
| └ | setMintMax | External ❗️ | 🛑  |NO❗️ |
| └ | mint | External ❗️ | 🛑  |NO❗️ |
| └ | mintBatch | External ❗️ | 🛑  |NO❗️ |
| └ | burn | External ❗️ | 🛑  |NO❗️ |
||||||
| **TheMallNft** | Implementation | ITheMallNft, KAP721 |||
| └ | <Constructor> | Public ❗️ | 🛑  | KAP721 |
| └ | exists | External ❗️ |   |NO❗️ |
| └ | tokenOfOwnerByPage | External ❗️ |   |NO❗️ |
| └ | tokenOfOwnerAll | External ❗️ |   |NO❗️ |
| └ | setTypeURI | External ❗️ | 🛑  | onlySuperAdmin |
| └ | setBaseURI | External ❗️ | 🛑  | onlyCommittee |
| └ | setMintMax | External ❗️ | 🛑  | onlySuperAdmin |
| └ | mint | External ❗️ | 🛑  | onlySuperAdmin |
| └ | mintBatch | External ❗️ | 🛑  | onlySuperAdmin |
| └ | burn | External ❗️ | 🛑  | onlySuperAdmin |
| └ | _mintInternal | Internal 🔒 | 🛑  | |


 Legend

|  Symbol  |  Meaning  |
|:--------:|-----------|
|    🛑    | Function can modify state |
|    💵    | Function is payable |
