### Project Milestones

#### December 2023

**Enhanced Test Coverage and Redemption Ratio:**

- Implemented improvements to test coverage, ensuring comprehensive testing of the codebase.
- Introduced a redemption ratio to enhance functionality related to redemptions.

**Code Optimization and Functional Additions:**

- Streamlined existing code for better efficiency.
- Implemented an Automated Market Maker (AMM) function to facilitate market operations.
- Optimized transaction limits for smoother processing.
- Added swapping functionality to support diverse trade scenarios.

**Branch Management and Documentation:**

- Successfully merged the 'main' branch into the local branch, aligning with the latest updates.
- Updated the project's README.md with swapping functionality details for improved documentation.

**Code Quality and Issue Resolution:**

- Proactively addressed and removed code warnings to enhance overall code quality.
- Resolved a critical 404 issue (fixed the design, a bug with buttons and the background itself, made the page more attractive) and fixed blog-related elements.

**Library Updates and Upgrades:**

- Managed updates for the 'o1js' library, ensuring compatibility with the latest enhancements.
- Updated various libraries, including 'tanstack,' removed 'iron-session,' and performed upgrades, including 'mina.'

**Test Expansion and Code Abstraction:**

- Expanded test coverage to validate a broader range of scenarios.
- Abstracted code for improved modularity, ensuring a scalable and maintainable codebase.

**Redeem Burns Implementation:**

- Committed changes related to redeem burns, contributing to the project's overall functionality.

#### January 2024

**Website Features and Design:**

- Implemented wallet functionality.
- Introduced new features and resolved screen-related issues.
- Enhanced the user experience with news-related features.
- Restructured the website by removing the Blog page and adding a News page.
- Resolved link-related issues and provided clear application instructions.

**Transaction and Notification System:**

- Implemented a notification system for successful transactions.
- Added footer and agreement functions for emails on the communication page.
- Fixed bugs affecting smaller screens.

**Contact Us Page:**

- Revamped the Contact Us page design.
- Introduced a new Contact Us form.

**Software Development Kit (SDK) and Smart Contract:**

- Continued development on the Software Development Kit (SDK).
- Added the deploy dex method and initiated tokens in the smart contract.
- Improved minting and deployment of 2 tokens.
- Conducted a thorough refactoring of logs.
- Implemented minor fixes and added SDK support for a token.
- Continued refining the token contract, separating balanceOf from minting.
- Created a dedicated function for initializing an address in the token contract.

**Interface Enhancements:**

- Resolved bugs affecting the mobile version.
- Improved the appearance of the pool page, allowing users to conveniently copy the address.
- Updated the interface for adding new pairs.

**Documentation:**

- Completely redesigned the documentation for user convenience and ease of learning.

**Other Updates:**

- Wrote a guide for connecting a wallet to the application.
- Updated our Twitter account with various information about our successes.

#### February 2024

**TradeCoin-mina NPM Package Refactor:**

- Included Berkeley testnet by adding Transaction Options, compiling contracts, and fetching accounts.
- Refactored dex into pair, pairMinting, and dex contracts.

**Smart Contract Improvements:**

- Added functions to manage reserves for 2 tokens, their addresses, and tree root information in the main pair contract.
- Implemented router Dex smart contract containing Merkle Trees for scaling and gas fee sponsorship.

**Frontend and Backend Enhancements:**

- Refactored frontend code into multiple components for better pool initialization and pair minting.
- Connected backend to the Mina Berkeley and Vercel Redis database.

**Wallet Function Updates:**

- Added functions to the wallet for hiding the address, copying the address, and disabling the wallet.
- Implemented a message system for failed wallet connections.

#### March 2024

**Smart Contract Method Additions:**

- Added a method for swapping base pool tokens.
- Implemented burning of LP tokens.
- Added explicit TypeScript in smart contracts and improved access control.

**Metadata and Database Improvements:**

- Created a script to add metadata and URI to the token.
- Developed a database schema for storing and accessing tokens allowed in Dex.
- Populated the Redis database with tokens data.

**Homepage and Interface Enhancements:**

- Improved homepage experience and interface for selecting a token.

#### April 2024

**Token Contract Extension:**

- Extended TokenContract with BasicTokenContract.

**Event and Error Management:**

- Added events and custom errors to three contracts.
- Implemented LP shares math and fee state for swapping and liquidity provision.
- Integrated Redis Vercel hashes storage.

**Research and Development:**

- Researched flash loans on Mina for off-chain implementation.
