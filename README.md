## Solidity Template

**Template for Solidity projects with a suite of useful tools pre-installed.**

## Tools used

- [foundry](https://github.com/foundry-rs/foundry): compiles, tests and deploys Solidity smart contracts
- [yarn](https://github.com/yarnpkg/yarn): manages project dependencies
- [prettier](https://github.com/prettier/prettier): formats non-Solidity files
- [solhint-community](https://github.com/solhint-community/solhint-community): lints Solidity smart contracts
- [husky](https://github.com/typicode/husky): runs git hooks
- [lint-staged](https://github.com/lint-staged/lint-staged): lints only staged files (in hooks)

> Note: Make sure `foundry` and `yarn` are installed before proceeding

## Recommended VSCode extensions

- [Prettier Formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
- [Solidity by Nomic Foundation](https://marketplace.visualstudio.com/items?itemName=NomicFoundation.hardhat-solidity)
- [EditorConfig](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)

## Github Actions

CI is preconfigured to:

1. check formatting and linting
2. build smart contracts
3. run tests
4. check test coverage percentage

## Installing Dependencies

While Foundry typically uses Git submodules to manage dependencies, this template opts for Node.js packages for better scalability.

To install dependencies:

1. Install an npm dependency:

```bash
yarn add dependency-name
```

1. Install a GitHub dependency:

```bash
yarn add github:username/repo-name#tag-branch-or-hash
```

2. Add the dependency to [remappings.txt](remappings.txt):

```bash
@openzeppelin/contracts/=node_modules/@openzeppelin/contracts/
forge-std/=node_modules/forge-std/src/
dependency-name=node_modules/dependency-name
```

> Note: [OpenZeppelin Contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) is pre-installed. You can follow its example for other dependencies.

## Useful commands

Build smart contracts:

```bash
yarn build
```

Clean build artifacts and cache :

```bash
yarn clean
```

Generate test coverage:

```bash
yarn coverage
```

Format files:

```bash
yarn fmt
```

Lint files:

```bash
yarn lint
```

Run tests:

```bash
yarn test
```

## Inspiration

This template is inspired by the following repositories:

- https://github.com/PaulRBerg/foundry-template
- https://github.com/OpenZeppelin/openzeppelin-contracts
- https://github.com/zkemail/email-recovery

## License

This project is licensed under MIT.
