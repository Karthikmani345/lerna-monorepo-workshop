# Lerna Monorepo Workshop 📚💡

This repository serves as an interactive workshop, focusing on managing and maintaining monorepos using Lerna. We cover topics ranging from managing multiple packages, independent versioning, to release management and change log generation.

## Pre-requisites 🛠

To get the most out of this workshop, you should have:

- A good understanding of JavaScript and Node.js.
- [Node.js](https://nodejs.org/en/download/) installed on your machine.
- [Yarn](https://classic.yarnpkg.com/en/docs/install) package manager installed.
- [Lerna](https://lerna.js.org/) installed globally via `npm install -g lerna`.

## Getting Started 🚀

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/karthikmani345/lerna-monorepo-workshop.git
   ```

2. Navigate to the project directory and install dependencies:

   ```bash
   cd lerna-monorepo-workshop
   lerna bootstrap
   ```

## Releasing and Publishing 🚀

The versioning and publishing of the packages are managed through GitHub actions. It's triggered when a pull request is merged into the `development` or `main` branch. The configuration for this can be found in the `.github/workflows` directory.

To simulate the versioning and publishing process locally, you can run the following commands:

- For pre-release (beta):

  ```bash
  npx lerna version --conventional-commits --conventional-prerelease --preid beta --yes --force-git-tag
  ```

- For final release:

  ```bash
  npx lerna version --conventional-commits --conventional-graduate --create-release github --yes --force-git-tag
  ```

(Note: the final release command also creates a GitHub release for the updated packages.)

## Workshop Structure 📚

The workshop is divided into modules, each focusing on different aspects of using Lerna with a monorepo:

- Module 1: Introduction to Monorepo and Lerna
- Module 2: Managing Multiple Packages
- Module 3: Independent Versioning
- Module 4: Release Management
- Module 5: Automating Change Log Generation

Each module contains a README with relevant information and exercises.

## Versioning 🏷

We use [Semantic Versioning](http://semver.org/) for all the packages in this repository. For the versions available, see the [tags on this repository](https://github.com/your-username/lerna-monorepo-workshop/tags).

## Contributing 🤝

We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to contribute.

## License 📄

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
