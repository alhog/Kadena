# Kadena & PACT

## Table of Contents

1. [Prerequisites](#prerequisites)
2. [Getting Started](#getting-started)
    - [Installation](#installation)
    - [Environment Variables](#environment-variables)
3. [Smart Contracts](#smart-contracts)
    - [Contract Addresses](#contract-addresses)
4. [Features](#features)
    - [Reading from the Chain](#reading-from-the-chain)
    - [Writing to the Chain](#writing-to-the-chain)
5. [Styling and UI](#styling-and-ui)
6. [Testing and Debugging](#testing-and-debugging)
7. [Deployment](#deployment)
    - [Deploying Smart Contracts](#deploying-smart-contracts)
    - [Deploying Your App](#deploying-your-app)
8. [Documentation and User Guides](#documentation-and-user-guides)
    - [Smart Contract Documentation](#smart-contract-documentation)
    - [User Guides](#user-guides)
9. [Contributing](#contributing)
10. [License](#license)

## Prerequisites

Before you begin, make sure you have the following installed:

- Node.js
- Pact compiler (for compiling your smart contracts)
- Chainweaver (for transaction signing and deployment)

## Getting Started

### Installation

1. Clone this repository:

    ```bash
    git clone https://github.com/your-username/your-kadena-dapp.git
    cd your-kadena-dapp
    ```

2. Install dependencies:

    ```bash
    npm install
    ```

### Environment Variables

Create a `.env` file in the root directory with the following variables:

- `REACT_APP_CHAINWEB_NODE_URL`: URL of the Kadena devnet or mainnet node.
- Other environment variables specific to your app (e.g., API keys).

## Smart Contracts

### Contract Addresses

- `coin.balance`: Address of the token balance contract.
- Other contract addresses used in your app.

## Features

### Reading from the Chain

- Use query functions to retrieve data from the blockchain.
- Example: Display account balances.

### Writing to the Chain

- Use command functions to modify the blockchain state.
- Example: Transfer tokens between accounts.

## Styling and UI

- Use CSS or styling libraries (e.g., Tailwind CSS, Bootstrap) for a consistent look.
- Design user-friendly forms, buttons, and navigation.

## Testing and Debugging

- Write unit tests for components and smart contracts.
- Debug using browser developer tools and Pact logging.

## Deployment

### Deploying Smart Contracts

1. Compile your Pact contract using the Pact compiler.
2. Deploy your contract to the Kadena devnet or mainnet.
3. Confirm deployment using the block explorer.

### Deploying Your App

1. Build your app for production.
2. Choose a hosting solution (e.g., Kadena devnet, Netlify, Vercel).
3. Configure environment variables.
4. Deploy your app.

## Documentation and User Guides

### Smart Contract Documentation

- Explain the purpose of each contract.
- Describe available functions and their usage.

### User Guides

- Provide installation instructions.
- Walk users through common tasks (e.g., transferring tokens).
- Include troubleshooting tips.

## Decentralized Apps
*Let's dive deeper into each of these steps and explore how they contribute to building your Kadena app:*

1. **CLI Tool and Integration**:
   - The **create-kadena-app CLI tool** is a powerful utility that streamlines the process of setting up your Kadena Blockchain application.
   - Here's what you need to know:
     - **Purpose**: The CLI tool kickstarts your project by creating the necessary project structure, setting up dependencies, and providing a foundation for your app.
     - **Typescript Integration**: The tool is designed to work seamlessly with Typescript, a statically typed superset of JavaScript. Typescript enhances code quality, readability, and maintainability.
     - **Dependencies**:
       - **@kadena/client**: This library allows your app to interact with the Kadena blockchain network programmatically. It provides functions for querying data, sending transactions, and more.
       - **@kadena/pactjs-cli**: Pact is Kadena's smart contract language. The pactjs-cli library enables you to interact with Pact contracts from your app.
     - **Benefits**: By using this CLI tool, you avoid manual setup and ensure consistency across Kadena projects.

2. **Smart Contract and Deployment**:
   - Your Kadena app includes a **smart contract** written in **Pact**.
   - Key points:
     - **Smart Contract**: A smart contract is a self-executing program that runs on the blockchain. It defines rules and logic for interactions.
     - **Pact Language**: Pact is specifically designed for Kadena. It offers security, formal verification, and expressiveness.
     - **Deployment**: Your smart contract is deployed on the Kadena Blockchain. This means it's live and ready to be used.
     - **Functional Application**: Having a deployed contract ensures that your app has a functional component right from the start.

3. **Common Use Cases Covered**:
   - The starter app addresses two common blockchain use cases:
     - **Reading a Message from the Chain**:
       - No transaction is needed.
       - You can directly retrieve information from the blockchain (e.g., querying an account balance).
     - **Writing a Message on the Chain**:
       - This involves a transaction.
       - You sign and send a transaction to the chain (e.g., transferring tokens).
       - You then wait for the transaction to be mined (confirmed) by the network.

4. **Chainweaver for Transaction Signing**:
   - **Chainweaver** is the official Kadena wallet.
   - Its role:
     - **Transaction Signing**: Chainweaver securely signs transactions before they are sent to the blockchain.
     - **Advanced Usage**: It's suitable for both regular users and developers working on smart contracts.
     - **User-Friendly Interface**: Chainweaver simplifies the process of interacting with the Kadena network.
    
   # Building an app
   Let's start by choosing a framework and setting up your Kadena project. This foundational step will determine the structure of your application and how you organize your code.

   *Here's how to proceed:*

## 1. Choose Your Framework

### Next.js
- **Description**: Next.js is a powerful React framework that provides server-side rendering (SSR) and static site generation (SSG). It's excellent for building performant web applications.
- **Key Features**:
  - Automatic code splitting for efficient loading.
  - Built-in routing system.
  - CSS modules support.
  - Hot module reloading (HMR) for a smooth development experience.
- **Use Cases**: Next.js is suitable for e-commerce sites, blogs, marketing pages, and complex web apps.

### Vue.js
- **Description**: Vue.js is a progressive JavaScript framework for building user interfaces. It's lightweight and easy to learn.
- **Key Features**:
  - Reactive data binding using a virtual DOM.
  - Component-based architecture.
  - Simple and intuitive syntax.
  - Official router (Vue Router) and state management (Vuex) libraries.
- **Use Cases**: Vue.js is great for creating interactive web apps, single-page applications (SPAs), and dynamic UI components.

### Angular
- **Description**: Angular is a comprehensive framework maintained by Google. It's suitable for large-scale, robust web applications.
- **Key Features**:
  - Full-featured framework with strong modularity.
  - TypeScript-based (static typing for JavaScript).
  - Powerful templating system.
  - Dependency injection for managing components and services.
- **Use Cases**: Angular is commonly used for enterprise apps, dashboards, and projects requiring extensive testing and scalability.

## 2. Setting Up Your Project

1. Install Node.js (if not already installed).
2. Open your terminal or command prompt.
3. Use the `create-kadena-app` CLI tool to create a new project:
   ```bash
   npx create-kadena-app my-kadena-app --template nextjs
   ```
   Replace `nextjs` with `vuejs` or `angular` if you choose a different framework.
4. Navigate to your project directory:
   ```bash
   cd my-kadena-app
   ```
5. Explore the generated project structure. You'll find folders for components, pages, styles, and other essential files.

# Project Structure 
 Understanding the organization of your Kadena app is crucial for efficient development. 
 
 *Here's what you'll find in your project directory:*

1. **`node_modules/`**:
   - This folder contains all the dependencies installed via npm (Node Package Manager). You don't need to manually manage this folder; npm handles it for you.

2. **`public/`**:
   - The `public` directory holds static assets that don't require processing (e.g., images, fonts, favicon.ico).
   - Files in this folder are directly accessible via URLs (e.g., `/favicon.ico`).

3. **`src/`**:
   - The heart of your application resides in the `src` folder.
   - Let's explore its subdirectories:

   - **`components/`**:
     - This folder houses reusable UI components.
     - Components can be buttons, forms, navigation bars, etc.
     - Organize components based on their functionality (e.g., `Header`, `Footer`, `Button`).

   - **`pages/`**:
     - Next.js-specific: This folder contains your application's pages.
     - Each `.js` or `.tsx` file in this directory corresponds to a route.
     - For example:
       - `pages/index.js` maps to the root URL (`/`).
       - `pages/about.js` maps to `/about`.

   - **`styles/`**:
     - Place your CSS or SCSS files here.
     - You can use global styles or component-specific styles.
     - Next.js supports CSS modules for scoped styling.

   - **`utils/`**:
     - Utility functions, helper classes, or constants go here.
     - Keep your code organized and reusable.

   - **`contracts/`**:
     - This is where your Pact smart contract files reside.
     - You'll find `.pact` files representing your contract logic.
     - Consider organizing contracts by functionality (e.g., `token.pact`, `nft.pact`).

   - **`services/`**:
     - If your app interacts with external APIs or services, place those interactions here.
     - For instance, a service that communicates with the Kadena blockchain using `@kadena/client`.

   - **`hooks/`**:
     - Custom React hooks can be defined here.
     - Hooks encapsulate logic (e.g., fetching data, managing state) and can be reused across components.

4. **`package.json`**:
   - This file contains metadata about your project and lists its dependencies.
   - It also includes scripts for running tasks (e.g., starting the development server, building the app).

5. **`tsconfig.json`** (if using TypeScript):
   - Configuration file for TypeScript.
   - Specifies compiler options, type checking rules, and project references.

6. **`README.md`**:
   - Your project's documentation.
   - Include information about how to run the app, its purpose, and any other relevant details.

Remember to explore each subdirectory further as you build your app. 

## Smart Contract Integration
Let's explore smart contract integration in your Kadena app. Smart contracts are the backbone of decentralized applications, enabling trustless interactions on the blockchain. 

*Here's how to integrate them:*

### Pact Smart Contracts
- **What is Pact?**
  - **Pact** is Kadena's smart contract language.
  - It's designed for security, formal verification, and ease of use.
  - Pact contracts run on the Kadena blockchain.

### Working with Pact Contracts
1. **Locate Your Contract File**:
   - In your project's `contracts/` directory, you'll find `.pact` files representing your smart contracts.
   - These files contain the contract logic, functions, and state transitions.

2. **Understanding Pact Contracts**:
   - Each contract defines a set of functions (also called capabilities).
   - Functions can:
     - Read data from the blockchain (query functions).
     - Modify the blockchain state (command functions).

3. **Query Functions**:
   - Query functions allow you to retrieve data from the blockchain without creating a transaction.
   - Example query function:
     ```pact
     (defun (balance {account : account}) 
       (at 'coin.balance {account}))
     ```
   - This function retrieves the balance of an account.

4. **Command Functions**:
   - Command functions modify the blockchain state.
   - Example command function:
     ```pact
     (defcap transfer
       (account : account)
       (amount : decimal)
       (to : account)
       (begin
         (coin.transfer {sender account} {to} {amount})
         (coin.transfer {to} {sender account} {amount})))
     ```
   - This function transfers tokens from one account to another.

5. **Deploying Contracts**:
   - Deploy your contract to the Kadena blockchain using Chainweaver or other deployment tools.
   - Once deployed, your contract is live and accessible by its name (e.g., `coin.balance`).

6. **Interacting with Contracts**:
   - In your app, use the `@kadena/client` library to call contract functions.
   - For example:
     ```javascript
     import { Pact } from '@kadena/client';

     const pact = new Pact({ node: 'https://api.chainweb.com/chainweb/0.0/mainnet01' });

     // Query balance
     const balance = await pact.fetch.local({
       pactCode: '(coin.balance {account "my-account"})',
     });

     // Execute transfer
     await pact.send.local({
       pactCode: '(coin.transfer {sender "my-account"} {to "recipient"} 100)',
     });
     ```

Remember to replace placeholders like `"my-account"` and `"recipient"` with actual account addresses. Also, ensure that your contract functions match the ones defined in your `.pact` files.

Feel free to explore your contract files, experiment with queries and commands, and integrate them into your app.
