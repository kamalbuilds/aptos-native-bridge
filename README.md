# aptos-native-bridge

Why users would like to use this as compared to existing bridging solutions ?

Building a bridge using Wormhole's Native Token Transfers (NTT) for Aptos offers several advantages over existing bridging solutions. Here’s a breakdown of why NTT might be a better option:

1. No Liquidity Pools Required
Traditional bridging methods rely on liquidity pools, which often lead to complications like slippage, front-running, and impermanent loss. NTT, on the other hand, bypasses these issues by not requiring liquidity pools. This reduces fees and the risk of MEV (Miner Extractable Value), which enhances efficiency and cost-effectiveness for users.

2. Native Token Transfers Over Wrapped Assets
With many existing bridges, users have to deal with wrapped tokens, which can create inconsistencies in token behavior across different chains. These wrapped tokens are usually owned by bridge contracts, limiting their flexibility and upgradeability. NTT allows you to transfer native tokens between chains directly, ensuring that tokens maintain their full functionality and behavior across all connected chains. This is critical when aiming for consistent cross-chain experiences and composability in DeFi applications.

3. Enhanced Security with Customizable Controls
NTT provides enhanced security by allowing custom rate limiting, access control, and attestation mechanisms. This enables integrators to define exactly how tokens are transferred, reducing risks like congestion and spam. Moreover, Wormhole’s Guardian Network, comprising 19 validators, secures NTT transfers, ensuring integrity across chains. In contrast, traditional bridges often rely on fewer security layers, making them more susceptible to vulnerabilities.

4. Flexibility in Token Management
NTT gives integrators full control over token contracts on each chain. This includes aspects like ownership, upgradeability, and token standards. This flexibility allows you to define custom rules for cross-chain token behavior, offering better adaptability for future needs or unforeseen requirements.

5. Seamless Cross-Chain Integration
NTT’s framework supports both burn-and-mint and hub-and-spoke models for token transfers, offering options that suit different deployment strategies. With the burn-and-mint mechanism, tokens are burned on the source chain and minted on the destination chain. This ensures that there is no double-counting of liquidity, a common issue with older bridging models.

6. Better Composability for DeFi Projects
For DeFi, especially on chains like Aptos, composability is key. NTT allows tokens to interact more naturally across multiple chains, enabling richer integrations without losing functionality or security. This makes NTT particularly attractive for cross-chain DeFi projects, as it enhances the overall user experience and operational efficiency.

Conclusion:
By using Wormhole's Native Token Transfers, we are leveraging a more secure, flexible, and cost-effective framework compared to traditional bridging methods. It provides better control over token functionality, avoids liquidity fragmentation, and enhances security with customizable features, making it a strong candidate for cross-chain projects on Aptos.
