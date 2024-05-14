# EEMT6000H-Intro-to-Blockchain
HKUST course project

#### Deploy the Contract
1. **Load the Contract:**
   - Create a new file in Remix and copy-paste your contract code or import the contract file directly.
  
2. **Compile the Contract:**
   - Navigate to the Solidity compiler tab, select the correct compiler version to match your contract's pragma (e.g., ^0.8.0), and click "Compile".

3. **Deploy the Contract:**
   - Enter any required constructor parameters (e.g., initial list of charity addresses).
   - Click "Deploy" and approve the transaction in MetaMask.

#### Interacting with the Contract
Once deployed, you can interact with the contract through the Remix interface under "Deployed Contracts".

1. **Add a Charity:**
   - Use the `addCharity` function if you need to add more charities post-deployment. Provide the charity's Ethereum address and confirm the transaction.

2. **Set Funding Goals:**
   - Select a charity and use the `setFundingGoal` function to set a funding goal (in Ether). This simulates setting a target for donations.

3. **Donate to Charities:**
   - Use the `donate` function to simulate sending donations. Enter arrays of charity addresses and corresponding amounts in Ether.
   - Ensure to send the exact total amount of Ether in the transaction value field in Remix.

4. **Check Funding Progress:**
   - Use the `checkFundingProgress` function by entering a charity's address to retrieve current funding status and the goal.

5. **Distribute Funds to Donees:**
   - As a charity, you can distribute funds to donees using the `distributeToDonee` function. Enter arrays of donee addresses and the amounts in Ether.
   - Ensure that the contract's balance covers the distribution and that the transaction value matches the total amount being distributed.

6. **Withdraw Funds:**
   - Charities can withdraw funds using the `withdrawFunds` function. Specify the amount in Ether and confirm the transaction.

7. **Request a Refund:**
   - Donors can request refunds for their donations using the `requestRefund` function. Provide the charity address from which the donation was made.

#### Observing Contract Events
- **Monitor Events:** Use Remix's logs to observe emitted events such as `DonationReceived`, `FundsDistributed`, and others to verify that the contract is functioning as expected during your tests.

#### Debugging
- **Use Remix Debugger:** Take advantage of Remix’s built-in debugger to trace transactions and fix issues in contract execution.

#### Finalizing Testing
- Review all interactions and ensure all functions behave as expected under various scenarios.
- Verify the final state of variables like balances and funding progress after conducting all operations.
