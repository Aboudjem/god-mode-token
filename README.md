# GodModeToken

This repository contains a smart contract for an ERC20 token called "GodModeToken", which allows the contract owner to transfer tokens between any addresses, bypassing the usual restrictions. The contract is based on the OpenZeppelin framework and licensed under UNLICENSED.

An ERC20 token is a standard for creating tokens on the Ethereum blockchain, it defines a set of rules that a token contract must follow in order to be considered an ERC20 token. These rules include a standard set of functions for transferring tokens, checking balances, and approving third-party transfers.

The "**GodModeToken**" contract inherits functionality from the OpenZeppelin "Ownable" and "ERC20" contracts. The "**Ownable**" contract provides an "**owner**" address, which is the address that deploys the contract and has special privileges, like the ability to call certain functions that other addresses cannot. The ERC20 contract provides all the standard function that an ERC20 token should have.

The contract's constructor initializes the token with a name and symbol, and also mints **100,000,000** tokens to the address that deploys the contract.

## Note

Be aware that the `transferFrom` function allows the contract owner to transfer tokens between any addresses, regardless of the restriction. Use this contract with caution and always review the code before using it.

Also, it is important to note that the contract is licensed under UNLICENSED, which means that the code is not associated with any open-source license. It means that the user of the contract should be aware of the legal implications of using this code.

## Scripts

This repository includes the following scripts in the `package.json` file:

### Test

`npm run test`

This command runs the test suite for the contract using the Hardhat testing framework. It will execute the command `npx hardhat test`, which will run all the tests in the project. The tests are used to check that the contract behaves as expected and to ensure that any changes made to the contract don't break existing functionality.

### Test with coverage

`npm run test:coverage`

This command runs the test suite and generates a coverage report for the contract. It will execute the command `npx hardhat coverage`, which will run all the tests in the project and also generate a coverage report. A coverage report shows how much of the contract's code is being executed by the test suite.

### Compile

`npm run compile`

This command compiles the contract using the Hardhat compiler. It will execute the command `npx hardhat compile`, which will compile the contract code, and generate the bytecode and ABI needed to deploy the contract on the Ethereum blockchain.

### Lint TypeScript

`npm run lint:ts`

This command runs the ESLint linter on all TypeScript files in the project. It will execute the command `npx eslint '**/*.ts'`, which will check all TypeScript files in the project against a set of linting rules and report any errors or warnings.

### Lint TypeScript and fix issues

`npm run lint:ts-fix`

This command runs the ESLint linter on all TypeScript files in the project and automatically fix any issues it finds.

### Lint Solidity

`npm run lint:sol`

This command runs the Prettier and Solhint linters on all the Solidity files in the project. It will execute the command `npx prettier '**/*.{json,sol,md}' --check && npx solhint 'contracts/**/*.sol'`, which will check all the solidity files in the project against a set of linting rules and report any errors or warnings.

### Lint Solidity and fix issues

`npm run lint:sol-fix`

This command runs the Prettier and Solhint linters on all the Solidity files in the project and automatically fix any issues it finds.

### Lint all

`npm run lint`

This command runs both TypeScript and Solidity linters in the project.

### Lint all and fix issues

`npm run lint:fix`

This command runs both TypeScript and Solidity linters in the project and automatically fix any issues it finds.

## Contribution

We welcome contributions to this repository. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.
