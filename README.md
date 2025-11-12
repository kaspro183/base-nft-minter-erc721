# Base NFT Minter — ERC721 + Metadata (Solidity + Hardhat + Frontend)

Projet prêt à publier sur GitHub pour montrer de l'activité **Web3/crypto** (parfait pour Talent Protocol).
- Réseau cible : **Base Sepolia** (testnet)
- Contrat : `MyNFT.sol` (ERC721 avec `tokenURI`)
- Frontend simple (HTML + JS + ethers.js) pour frapper un NFT avec une **URI de metadata**

> Pas besoin de déployer pour Talent Protocol — **les commits GitHub suffisent**.  
> Pour tester la dApp, déployez sur **Base Sepolia** puis configurez `frontend/app.js`.

## Structure
```
base-nft-minter-erc721/
├── contracts/MyNFT.sol
├── scripts/deploy.js
├── hardhat.config.js
├── package.json
└── frontend/
    ├── index.html
    └── app.js
```

## Déploiement (optionnel)
```bash
npm i
npx hardhat compile

# Variables d'env pour Base Sepolia
# export BASE_SEPOLIA_RPC="https://sepolia.base.org"
# export PRIVATE_KEY="0x..."
npx hardhat run scripts/deploy.js --network base_sepolia
```

## Frontend (après déploiement)
- Ouvrez `frontend/app.js` et remplacez `const NFT_ADDRESS = "0xYourNFT";`
- Ouvrez `frontend/index.html` (MetaMask + réseau **Base Sepolia**).
