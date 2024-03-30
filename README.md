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
