# Advanced-Solidity

1. Created the KaseiCoin Token Contract that defines KaseiCoin as an ERC-20 token
    * Imported the provided KaseiCoin.sol starter file into the Remix IDE.
    * Imported the following contracts from the OpenZeppelin library:ERC20, ERC20Detailed, ERC20Mintable
    * Defined a contract for the KaseiCoin token, and named it KaseiCoin. Havd the contract inherit the three contracts that were imported from OpenZeppelin.
    * Inside the KaseiCoin contract, added a constructor with the following parameters: name, symbol, and initial_supply.
    * As part of the constructor definition, added a call to the constructor of the ERC20Detailed contract, passing the parameters name, symbol, and 18. 
    * Compiled the contract by using compiler version 0.5.0.
    * Screenshot of the compilation of the contract:
![image](https://github.com/nhc12/Advanced-Solidity/blob/main/Execution_Results/Successful%20compilation%20of%20the%20contract%20KaseiCoin.jpg)

2. Created the KaseiCoin Crowdsale Contract: 
    * Imported the provided KaseiCoinCrowdsale.sol starter code into the Remix IDE.
    * Inherited the following OpenZeppelin contracts: Crowdsale, MintedCrowdsale
    * In the KaisenCoinCrowdsale constructor, provided parameters for all the features of the crowdsale, such as rate, wallet and token. 
    * Compiled the contract by using compiler version 0.5.0.
    * Screenshot of the compilation of the contract: 
![image](https://github.com/nhc12/Advanced-Solidity/blob/main/Execution_Results/Successful%20compilation%20of%20the%20contract%20KaseiCoinCrowdsale.jpg)

3. Created the KaseiCoin Deployer Contract: 
    * Uncommented the KaseiCoinCrowdsaleDeployer contract in the provided KaseiCoinCrowdsale.sol starter code.
    * Added variables to store the addresses of the KaseiCoin and KaseiCoinCrowdsale contracts, which this contract will deploy.
    * Complete the KaseiCoinCrowdsaleDeployer contract by:
       * Created an address public variable named kasei_token_address, which will store the KaseiCoin address once that contract has been deployed. 
       * Created an address public variable named kasei_crowdsale_address, which will store the KaseiCoinCrowdsale address once that contract has been deployed.
       * Added the following parameters to the constructor for the KaseiCoinCrowdsaleDeployer contract: name, symbol, and wallet.
       * Completed the Constructor: rate, wallet, token
       * Assigned the address of the KaseiCoin crowdsale contract to the kasei_crowdsale_address variable.
       * Set the KaseiCoinCrowdsale contract as a minter.
       * Had the KaseiCoinCrowdsaleDeployer renounce its minter role.
       * Compiled the contract by using compiler version 0.5.0.
       * Screenshot of the compilation of the contract: 
![image](https://github.com/nhc12/Advanced-Solidity/blob/main/Execution_Results/Deployed%20Contract.jpg)

4. Deployed and Tested the Crowdsale on a Local Blockchain: 
    * Deployed the crowdsale to a local blockchain by using Remix, MetaMask, and Ganache:
![image](https://github.com/nhc12/Advanced-Solidity/blob/main/Execution_Results/Deployed%20the%20crowdsale%20to%20a%20local%20blockchain%20by%20using%20Remix%2C%20MetaMask%2C%20and%20Ganache..jpg)
    * Test the functionality of the crowdsale by using test accounts to buy new tokens and then checking the balances of those accounts:
![image](https://github.com/nhc12/Advanced-Solidity/blob/main/Execution_Results/Test%20the%20functionality%20of%20the%20crowdsale%20by%20using%20test%20accounts%20to%20buy%20new%20tokens%20and%20then%20checking%20the%20balances%20of%20those%20accounts.jpg)
    * Reviewed the total supply of minted tokens and the amount of wei that the crowdsale contract has raised:
![image](https://github.com/nhc12/Advanced-Solidity/blob/main/Execution_Results/Review%20the%20total%20supply%20of%20minted%20tokens%20and%20the%20amount%20of%20wei%20that%20the%20crowdsale%20contract%20has%20raised..jpg)

5. Attachmnents:
      * Starter Codes (KaseiCoin.sol and KaseiCoinCrowdsale.sol)
      * Codes for deployment .txt 
      * Screenshots of Deployment 
       
       
       
       
       
       
       
       
       
       




