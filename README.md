# erc404plus

===================================================================================================

Main Conclusion: Our newly developed ERC404+ standard addresses and resolves the significant issue present in the current ERC404 standard, where NFT IDs can exceed the total supply limit. This not only maintains the aesthetic integrity of the NFT IDs but also enhances security by preventing potential exploits.

Supporting Arguments: Problem with Current ERC404 Standard: In existing ERC404 implementations, there is a discrepancy where the total supply of NFTs might be capped (e.g., 10,000), yet the IDs assigned to NFTs can exceed this total supply (e.g., reaching 13,213 IDs for a project supposed to have 8,000 NFTs). This mismatch is not just a matter of poor aesthetics but poses a security risk, potentially allowing exploiters to manipulate or steal NFTs based on the inflated ID range.

Our Solution - ERC404+: To counteract this problem, our ERC404+ standard introduces a novel mechanism. We've added a _burnedTokenIds array that keeps track of all IDs from burned (or destroyed) NFTs. Once the total supply limit is reached through minting, our contract design recycles IDs from the _burnedTokenIds array for new NFTs, thereby ensuring that no new ID exceeds the total supply limit. This approach not only keeps the ID sequence within the intended range but also effectively brings "dead" NFTs back to life by reusing their IDs for new issues.

Benefits of ERC404+: Aesthetic Integrity: By ensuring that NFT IDs do not surpass the total supply, we maintain a coherent and predictable numbering system that aligns with the project's scope. Enhanced Security: The mechanism significantly reduces the risk of exploits related to ID manipulation, as there's no longer an inflated range of IDs beyond the total supply. Resource Optimization: Recycling IDs from burned NFTs is an efficient use of resources, allowing for the revitalization of these IDs and ensuring that the total NFT ecosystem remains within its intended bounds.

Conclusion: The introduction of ERC404+ marks a significant advancement over the current ERC404 standard, addressing both aesthetic concerns and security vulnerabilities associated with NFT ID management. By implementing a system that recycles IDs from burned NFTs, we ensure that NFT IDs remain within the total supply limit, thus reinforcing the integrity and security of the NFT ecosystem. This innovative approach demonstrates our commitment to improving NFT standards and enhancing the overall user and developer experience in the blockchain space.

===================================================================================================

The full code will be posted soon in this repo. $FORGE
