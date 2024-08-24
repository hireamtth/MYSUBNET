### Creating and Managing an EVM Subnet with Ava Labs on Avalanche

Welcome to the guide on setting up your EVM Subnet on Avalanche using Ava Labs tools. This guide will help you create an EVM Subnet, deploy it, and connect it with Metamask. Additionally, we'll cover how to deploy ERC-20 and Vault contracts on your subnet and provide a README file to help you get started.

---

## **1. Create and Deploy Your EVM Subnet**

### **Step-by-Step Instructions:**

1. **Install Avalanche CLI Tool:**
   - To interact with the Avalanche network, install the Avalanche Command Line Interface (CLI) tool. Follow the installation instructions in the [official documentation](https://docs.avax.network/build/avalanchego-developing/avalanche-cli).

2. **Create a New Subnet:**
   - Run the command to create a new subnet:
     ```bash
     avalanche subnet create mySubnet
     ```
   - Follow the prompts:
     ```
     Enter your subnet's ChainId. It can be any positive integer.
     ChainId: 12345567
     Select a symbol for your subnet's native token
     Token symbol: MYSUBNET
     ```

3. **Deploy the Subnet:**
   - Deploy your subnet using:
     ```bash
     avalanche subnet deploy mySubnet
     ```

4. **View Subnet Details:**
   - After deployment, view your subnet details in the console.

5. **Connect to Metamask:**
   - Use the provided RPC URL and chain details to connect your subnet to Metamask.
   - **RPC URL:** `http://127.0.0.1:9650/ext/bc/SPqou41AALqxDquEycNYuTJmRvZYbfoV9DYApDJVXKXuwVFPz/rpc`
   - **Funded Address:** `0x8db97C7cEcE249c2b98bDC0226Cc4C2A57BF52FC`
   - **Private Key:** `56289e99c94b6912bfc12adc093c9b51124f0dc54ac7a766b2bc5ccf558d8027`
   - **Network Name:** `mySubnet`
   - **Chain ID:** `54325`
   - **Currency Symbol:** `TUTORIAL`

   To add the network to Metamask:
   - Open Metamask and go to **Networks** > **Add a network** > **Add a network manually**.
   - Enter the details and click **Save**.

6. **Stop the Subnet:**
   - When finished, stop the subnet with:
     ```bash
     avalanche network stop
     ```

2. **Compile and Deploy the Contract:**
   - Use [Remix IDE](https://remix.ethereum.org/) to compile and deploy the contract on your subnet.
   - Alternatively, use Truffle or Hardhat to deploy from your local development environment.


2. **Compile and Deploy the Contract:**
   - As with the ERC-20 contract, use Remix, Truffle, or Hardhat to compile and deploy the Vault contract on your subnet.

---

## **README File**

```markdown
# EVM Subnet Setup and Contract Deployment on Avalanche

## **1. Creating and Deploying Your EVM Subnet**

Follow these steps to create and deploy an EVM Subnet using the Avalanche CLI:

1. **Install Avalanche CLI Tool:**
   - Follow the [official installation guide](https://docs.avax.network/build/avalanchego-developing/avalanche-cli).

2. **Create a New Subnet:**
   ```bash
   avalanche subnet create mySubnet
   ```

3. **Deploy the Subnet:**
   ```bash
   avalanche subnet deploy mySubnet
   ```

4. **View Subnet Details:**
   - Check the details in the console.

5. **Connect to Metamask:**
   - **RPC URL:** `http://127.0.0.1:9650/ext/bc/SPqou41AALqxDquEycNYuTJmRvZYbfoV9DYApDJVXKXuwVFPz/rpc`
   - **Funded Address:** `0x8db97C7cEcE249c2b98bDC0226Cc4C2A57BF52FC`
   - **Private Key:** `56289e99c94b6912bfc12adc093c9b51124f0dc54ac7a766b2bc5ccf558d8027`
   - **Network Name:** `mySubnet`
   - **Chain ID:** `54325`
   - **Currency Symbol:** `TUTORIAL`
   - Add these details to Metamask under **Networks** > **Add a network**.

6. **Stop the Subnet:**
   ```bash
   avalanche network stop
   ```

2. **Deploy the Contract:**
   - Compile and deploy using Remix

## **Additional Resources**

- [Avalanche Documentation](https://docs.avax.network/)
- [OpenZeppelin Contracts](https://docs.openzeppelin.com/contracts/4.x/)

## Contact 
prajwalhiremath021@gmail.com
