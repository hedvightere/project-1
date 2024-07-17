# Welcome to the Crypto Kingdom 🏰

## Chapter 1: The Tale of the ERC20 Token 🪙

In the faraway land of the Blockchain, there existed a magical token called **ERC20**. This token had the power to be transferred, approved, and spent across the kingdom. Let’s dive into its enchanted functionalities.

### ERC20: The Royal Treasury

**Contract Name:** `ERC20Token.sol`

### The Scroll of Declarations

#### Magical Spells (Functions)

1. **Total Supply (`totalSupply`)**
   - **Spell Description:** Reveals the total number of tokens in existence.
   - **Invocation:** `totalSupply() public view returns (uint256)`

2. **Balance of (`balanceOf`)**
   - **Spell Description:** Shows the token balance of a given account.
   - **Invocation:** `balanceOf(address account) public view returns (uint256)`

3. **Transfer (`transfer`)**
   - **Spell Description:** Moves tokens from the sender to a recipient.
   - **Invocation:** `transfer(address recipient, uint256 amount) public returns (bool)`

4. **Approve (`approve`)**
   - **Spell Description:** Grants permission to spend a specified amount of tokens on behalf of the sender.
   - **Invocation:** `approve(address spender, uint256 amount) public returns (bool)`

5. **Transfer From (`transferFrom`)**
   - **Spell Description:** Moves tokens from one account to another using an allowance.
   - **Invocation:** `transferFrom(address sender, address recipient, uint256 amount) public returns (bool)`

6. **Allowance (`allowance`)**
   - **Spell Description:** Shows the remaining tokens that a spender is allowed to spend on behalf of an owner.
   - **Invocation:** `allowance(address owner, address spender) public view returns (uint256)`

### Enchantments (Events)

- **Transfer (Emits when tokens are transferred)**
  ```solidity
  event Transfer(address indexed from, address indexed to, uint256 value);
  ```

- **Approval (Emits when a successful call to `approve` is made)**
  ```solidity
  event Approval(address indexed owner, address indexed spender, uint256 value);
  ```

## Chapter 2: The Vault of Fortunes 💰

Nestled deep within the Blockchain Kingdom lies the **Vault**. This Vault securely holds treasures and releases them only to the worthy.

### Vault: The Guardian of Riches

**Contract Name:** `Vault.sol`

### The Scroll of Declarations

#### Sacred Keys (Functions)

1. **Deposit (`deposit`)**
   - **Key Description:** Safely locks away tokens into the Vault.
   - **Invocation:** `deposit(uint256 amount) public`

2. **Withdraw (`withdraw`)**
   - **Key Description:** Releases a specified amount of tokens to the caller.
   - **Invocation:** `withdraw(uint256 amount) public`

3. **Check Balance (`checkBalance`)**
   - **Key Description:** Reveals the caller’s balance within the Vault.
   - **Invocation:** `checkBalance() public view returns (uint256)`

4. **Total Deposits (`totalDeposits`)**
   - **Key Description:** Discloses the total tokens stored within the Vault.
   - **Invocation:** `totalDeposits() public view returns (uint256)`

### Enchantments (Events)

- **Deposit (Emits when tokens are deposited into the Vault)**
  ```solidity
  event Deposit(address indexed user, uint256 amount);
  ```

- **Withdraw (Emits when tokens are withdrawn from the Vault)**
  ```solidity
  event Withdraw(address indexed user, uint256 amount);
  ```

=
