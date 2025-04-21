# CosmoList RPC Submission

## Description
This repository allows contributors to submit their RPC endpoints for various blockchain networks. You can create a pull request to add your RPC to the appropriate configuration file, and it will be reviewed for inclusion.

---

## How to Add Your RPC
- Use `https://` we use only this format for greater security

1. **Fork this repository**:
   - Click the `Fork` button in the top-right corner of this page.

2. **Clone your forked repository**:
   ```bash
   https://github.com/R1M-NODES/cosmolist.git
   cd cosmolist
   ```

3. **Navigate to the appropriate file**:
   - For example, if you want to add an RPC for Celestia Mainnet, navigate to:
     ```
     public/celestia/mainnet/js/rpc-config.js
     ```

4. **Add your RPC**:
   - Open the file and add your RPC URL to the `rpcServers` array in the following format:
     ```javascript
     export const rpcServers = [
         "https://celestia-rpc.stake-town.com",
         "https://celestia-mainnet-rpc.itrocket.net",
         "https://celestia.rpc.kjnodes.com",
         "https://your-rpc-url.com", // Add your RPC here
         ...existing RPCs...
     ];
     ```

5. **Commit your changes**:
   ```bash
   git add .
   git commit -m "Add my RPC endpoint for Celestia Mainnet"
   ```

6. **Push your changes to your fork**:
   ```bash
   git push origin main
   ```

7. **Create a pull request**:
   - Go to your forked repository on GitHub.
   - Click the `Compare & pull request` button.
   - Provide a description of your changes and click `Create pull request`.

---

## RPC Format
Your RPC should follow this format:
- Use `https://` we use only this format for greater security
- **Example**:
  ```javascript
  "https://your-rpc-url.com"
  ```

---

## Example of `rpc-config.js`
Here’s an example of how the `rpc-config.js` file should look after adding your RPC:
```javascript
export const rpcServers = [
    "https://celestia-rpc.stake-town.com",
    "https://celestia-mainnet-rpc.itrocket.net",
    "https://celestia.rpc.kjnodes.com",
    "https://your-rpc-url.com" // Your added RPC
];
```
