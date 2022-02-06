# Drizzle + Truffle + React Simple Storage dApp

dApp that stores & retrieves a value from an Ethereum Smart Contract. Built with Solidity Truffle framework and Drizzle React+Redux libraries


# How to run

1.  Run the development console.
    
    `truffle develop` 
    
2.  Compile and migrate the smart contracts. Note inside the development console we don't preface commands with  `truffle`.
    
    `compile`
    `migrate` 
    
3.  In the  `app`  directory, we run the React app. Smart contract changes must be manually recompiled and migrated.
    
    `// in another terminal (i.e. not in the truffle develop prompt)`
    `cd app`
    `npm run start` 
    
4.  Truffle can run tests written in Solidity or JavaScript against your smart contracts. Note the command varies slightly if you're in or outside of the development console.
    
    `// inside the development console`
    `test`
    
    `// outside the development console`
    `truffle test` 
    
5.  Jest is included for testing React components. Compile your contracts before running Jest, or you may receive some file not found errors.
    
    `// ensure you are inside the app directory when running this`
    `npm run test` 
    
6.  To build the application for production, use the build script. A production build will be in the  `app/build`  folder.
    
    `// ensure you are inside the app directory when running this`
    `npm run build`
