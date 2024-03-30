# Kadena & PACT



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
