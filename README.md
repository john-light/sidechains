# About
This project attempts to create a comprehensive list of resources related to sidechain design and development.

## Terminology
According to the original [sidechains whitepaper](https://blockstream.com/sidechains.pdf) by Back et al, a sidechain is:

> a blockchain that validates data from other blockchains (p. 8)

An example of a sidechain under this definition would be Ethereum, a blockchain that can validate data from the bitcoin blockchain in the form of [SPV proofs](https://medium.com/summa-technology/cross-chain-auction-technical-f16710bfe69f).

Back et al go on to define a pegged sidechain as:

> a sidechain whose assets can be imported from and returned to other chains; that is, a sidechain that supports two-way pegged assets. (p.8)

The blockchain that an asset is imported from is the "mainchain" or "parent chain", and the blockchain that the asset is imported to is the sidechain. The mutual portability between a mainchain and a sidechain is referred to as a "two-way peg" due to the way that the value of an asset is "pegged" 1:1 when minted on a sidechain i.e. a pegged asset minted on a sidechain should always be redeemable 1:1 (minus any fees) for the asset it represents on the mainchain.

Thus, crucial to the definition of a pegged sidechain, in the author's humble opinion, is that the portability of assets between a mainchain and sidechain should be permissionless; that is, no permission from any third part(y)(ies) should be required to import an asset into and export an asset from a sidechain. Back et al say as much as well:

> 1. Assets which are moved between sidechains should be able to be moved back by whomever their current holder is, and nobody else (including previous holders).  
> 2. Assets should be moved without counterparty risk; that is, there should be no ability for a dishonest party to prevent the transfer occurring. (p. 5)  

Taken together, we can say that a pegged sidechain is:

> a blockchain that validates data from other blockchains and supports permissionless, counterparty-free two-way pegged assets.  

Based on observations by the author, this is the definition that most people probably think of when they use the term "sidechains", as opposed to the older and simpler definition given by Back et al. And so, while technically what is being referred to here is a "pegged sidechain", the same concept is now colloquially referred to simply as "sidechain" and this is how the term is used in this project as well.

# Papers

- 2014-10-22: [Enabling Blockchain Innovations with Pegged Sidechains](https://blockstream.com/sidechains.pdf)  

- 2016-04-01: [Drivechains, Sidechains and Hybrid 2-way peg Designs](https://docs.rsk.co/Drivechains_Sidechains_and_Hybrid_2-way_peg_Designs_R9.pdf)  

- 2017-08-21: [Merged Mining: Curse of Cure?](https://eprint.iacr.org/2017/791)  

- 2017-09-05: [Driveproof: Sidechain Headers On Mainchain (SHM)](https://zmnscpxj.github.io/sidechain/driveproof/index.html)  

- 2017-09-23: [Proof-of-mainstake](https://zmnscpxj.github.io/sidechain/mainstake/index.html)  

- 2017-12-02: [Sidechain Weaknesses](https://zmnscpxj.github.io/sidechain/weakness/index.html)  

- 2018-06-28: [Research of Merged Mining Technology in Bitcoin Blockchain Scaling](http://www.wcse.org/WCSE_2018/W072.pdf)  

- 2018-07-03: [CountAcks Drivechain](https://github.com/rsksmart/bips/blob/master/BIP-R11.md)  

- 2018-10-17: [Sidechains: Decoupled Consensus Between Chains](https://www.horizen.io/assets/files/Horizen-Sidechains-Decoupled-Consensus-Between-Chains.pdf)  

- 2018-10-30: [Proof-of-Work Sidechains](https://eprint.iacr.org/2018/1048.pdf)  

- 2018-12-18: [Proof-of-Stake Sidechains](https://eprint.iacr.org/2018/1239.pdf)  

- 2019-01-18: [Proof-of-Stake Bitcoin Sidechains](https://github.com/nomic-io/bitcoin-peg/blob/master/bitcoinPeg.md)  

- 2020-01-01: [Zendoo: a zk-SNARK Verifiable Cross-Chain Transfer Protocol Enabling Decoupled and Decentralized Sidechains](https://eprint.iacr.org/2020/123.pdf)  
- 2020-11-12: [Horizon: A Gas-Efficient Trustless Bridge for Cross-Chain Transactions](https://harmony.one/crosschain.pdf)  

- 2020-12-31: [Softchains: Sidechains as a Soft Fork via Proof-of-Work Fraud Proofs](https://gist.github.com/RubenSomsen/7ecf7f13dc2496aa7eed8815a02f13d1)  

# Blog posts

- 2014-10-26: [A simple explanation of Bitcoin "Sidechains"](https://gendal.me/2014/10/26/a-simple-explanation-of-bitcoin-sidechains/)  

- 2015-04-10: [Pegged Sidechains Whitepaper Notes](http://kevinriggen.com/Bitcoin/2015-04-10-Pegged-Sidechains-Whitepaper-Notes)  

- 2015-11-24: [Drivechain - The Simple Two Way Peg](https://www.truthcoin.info/blog/drivechain/)  

- 2017-01-30: [Blind Merged Mining](https://www.truthcoin.info/blog/blind-merged-mining/)  

- 2018-08-30: [Ion Stage 2: Toward a General Interoperability Protocol (Part 1)](https://medium.com/clearmatics/ion-stage-2-toward-a-general-interoperability-protocol-part-1-d12b9d7316d3)  

- 2019-04-17: [Why Drivechain Is Harder to Understand Than Previous Soft Forks](https://www.drivechain.info/blog/hard-to-understand/)  

- 2019-04-17: [Is Liquid A "Real" Sidechain? Greg Maxwell Weighs In](https://www.drivechain.info/blog/liquid/)  

- 2019-12-10: [Blind Merged Mining with covenants ( sighash_anyprevout / op_ctv )](https://gist.github.com/RubenSomsen/5e4be6d18e5fa526b17d8b34906b16a5)  

- 2020-04-30: [The difference between XCAT and Drivechain](https://lightco.in/2020/04/30/xcat-drivechain/)  

- 2020-08-02: [Comparing two-way bitcoin pegs](https://lightco.in/2020/08/02/bitcoin-pegs/)  

- 2020-11-08: [Scaling bitcoin with sidechains](https://lightco.in/2020/11/08/sidechains/)  

# Discussion threads

- 2014-04-12: [Why do people think that side-chains are going to be secure?](https://www.reddit.com/r/Bitcoin/comments/22vn4m/why_do_people_think_that_sidechains_are_going_to/)  

- 2014-10-23: [Sidechains whitepaper AMA](https://www.reddit.com/r/IAmA/comments/2k3u97/we_are_bitcoin_sidechain_paper_authors_adam_back/)  

- 2014-12-20: [The relationship between Proof-of-Publication and Anti-Replay Oracles](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2014-December/007029.html)  

- 2016-10-02: [Drivechain proposal using OP_COUNT_ACKS](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2016-October/013174.html)  

- 2017-02-24: [How an anchored Proof of Stake Sidechain can help the Bitcoin main chain](https://www.reddit.com/r/Bitcoin/duplicates/5vy4qc/how_an_anchored_proof_of_stake_sidechain_can_help/)  

- 2017-06-10: [Drivechain -- Request for discussion](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2017-June/014558.html)  

- 2017-07-10: [Updating the Scaling Roadmap](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2017-July/014718.html)  

- 2017-09-05: [Sidechain headers on mainchain (unification of drivechains and spv proofs)](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2017-September/014910.html)  

- 2017-09-23: [Sidechains: Mainstake](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2017-September/015045.html)  

- 2017-12-01: [Two Drivechain BIPs](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2017-December/015339.html)  

- 2018-01-17: [NiPoPoW criticism](https://twitter.com/peterktodd/status/953511085008609280)  

- 2019-07-04: [SIDECHAINS ARE NOT LAYER 2](https://twitter.com/gakonst/status/1146793685545304064)  

- 2020-12-31: [Softchains: Sidechains as a Soft Fork via Proof-of-Work Fraud Proofs](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2020-December/018331.html)  

# Presentations

- 2015-current: [Drivechain presentations](https://www.drivechain.info/literature/index.html)  

- 2015-06-28: [SF Bitcoin Devs Seminar: Sidechains: Bringing New Elements to Bitcoin](https://youtu.be/Twynh6xIKUc)  

- 2018-10-17: [Horizen Sidechains: Decoupled Consensus Between Chains](https://youtu.be/HzuJ48zyhKU)  

- 2019-04-18: [Proof-of-Stake Sidechains for Cardano](https://docs.google.com/presentation/d/17x25AfvnMOpmXFO7wqs5q0AtW4yrYJeVPS2Lb22thyo/edit#slide=id.g5118426647_0_0)  

# Interviews

- 2015-08-17: [Sidechains and Lightning Networks with Rusty Russell](https://softwareengineeringdaily.com/2015/08/17/sidechains-and-lightning-networks-with-rusty-russell/)  

- 2016-04-19: [Interview with Greg Maxwell: Lightning Network Better Than Sidechains for Scaling Bitcoin](https://bitcoinmagazine.com/articles/greg-maxwell-lightning-network-better-than-sidechains-for-scaling-bitcoin-1461077424)  

- 2017-11-15: [Daniel Krawisz and Paul Sztorc talk Drivechain](https://www.youtube.com/watch?v=iMNLB7Q8z80)  

- 2018-09-30: [Let's Talk Bitcoin! #377 Sidechains, Drivechains and the Apple Store](https://letstalkbitcoin.com/blog/post/lets-talk-bitcoin-377-sidechains-drivechains-and-the-apple-store)  

- 2020-08-27: [Cosmos Unchained: Bitcoin Peggy Showdown](https://www.youtube.com/watch?v=ArSftVH1Ads)  

- 2020-09-17: [How Bitcoin Sidechains are the Altcoin Killer! An Interview with Paul Sztorc on Drivechains](https://youtu.be/BbcIAaWScUc)  

# News

- 2014-04-16: [Side Chains: The How, The Challenges and the Potential](https://bitcoinmagazine.com/articles/side-chains-challenges-potential)  

- 2014-10-23: [Sidechains White Paper Imagines New Future for Digital Currency Development](https://www.coindesk.com/sidechains-white-paper-ecosystem-reboot)  

- 2014-10-25: [Bitcoin 2.0: Sidechains And Ethereum And Zerocash, Oh My!](https://techcrunch.com/2014/10/25/bitcoin-2-0-sidechains-and-zerocash-and-ethereum-oh-my/)  

- 2017-06-05: [Are Sidechains a Better Solution for Bitcoin’s Scaling Debate?](https://www.coindesk.com/are-sidechains-a-better-solution-for-bitcoins-scaling-debate)  

- 2018-01-17: [The Sidechains Breakthrough Almost Everyone in Bitcoin Missed](https://www.coindesk.com/sidechains-breakthrough-almost-everyone-bitcoin-missed)  

- 2018-02-19: [Sidechains: Why These Researchers Think They Solved a Key Piece of the Puzzle](https://bitcoinmagazine.com/articles/sidechains-why-these-researchers-think-they-solved-key-piece-puzzle)  

- 2018-09-25: [Bitcoin Takes a Step Toward Becoming a ‘Multi-Network’ Cryptocurrency](https://www.coindesk.com/bitcoin-just-took-a-step-toward-becoming-a-multi-network-cryptocurrency)  

- 2019-02-27: [It's 2019, Where Are Bitcoin's Sidechains?](https://www.forbes.com/sites/ktorpey/2019/02/27/its-2019-where-are-bitcoins-sidechains/#7d917c553b4f)  

- 2020-12-08: [RSK Is Evolving; Powpeg Leverages Hash Power To Switch From Bitcoin To Sidechain And Back](https://bitcoinmagazine.com/articles/rsk-is-evolving-powpeg-leverages-hash-power-to-switch-from-bitcoin-to-sidechain-and-back)  

# Patents

- 2018-03-27: [Transferring ledger assets between blockchains via pegged sidechains](https://patents.google.com/patent/US20160330034A1/en)  

# Semi-related
While not directly related to sidechains _per se_, the following resources may be useful to understand the design space and tradeoffs around sidechains, and may describe complementary technologies as well.

## Centralized pegs

- 2019-01-24: [Wrapped Tokens: A multi-institutional framework for tokenizing any asset](https://wbtc.network/assets/wrapped-tokens-whitepaper.pdf)

- 2019-07-09: [HTLC and Atomic Peg](https://github.com/bnb-chain/BEPs/blob/master/BEP3.md)

## Collateralized pegs

- 2018-10-15: [Retrofitting a two-way peg between blockchains](https://arxiv.org/pdf/1908.03999.pdf)

- 2019-03-15: [XCLAIM: Trustless, Interoperable, Cryptocurrency-Backed Assets](https://eprint.iacr.org/2018/643.pdf)  

- 2019-08-16: [tBTC: A Decentralized Redeemable BTC-backed ERC-20 Token](https://docs.keep.network/tbtc/)  

- 2020-05-02: [Zcash Pegzone v2](https://github.com/ZcashFoundation/zcash-pegzone/blob/f8e22c4f9345d71256f98cd5d192e17de4c9b1dc/README.md)  

- 2020-10-06: [Decentralized Custody Scheme with Game-Theoretic Security](https://arxiv.org/pdf/2008.10895.pdf)  

- 2020-10-08: [Introducing the Wormhole Bridge](https://medium.com/certus-one/introducing-the-wormhole-bridge-24911b7335f7)  

- 2021-01-XX: [Axelar Network: Connecting Applications with Blockchain Ecosystems](https://static1.squarespace.com/static/5f7679246f2afb311bbb67dd/t/602d3503ad35b40d1bdc209c/1613575428020/axelar_whitepaper_v1.pdf)  

- 2021-01-25: [Introducing StakePeg: A trust-reduced two-way bitcoin peg](https://lightco.in/2021/01/25/stakepeg/)  

- 2021-02-25: [How Gravity works](https://blog.althea.net/how-gravity-works/)  

- 2021-09-13: [Optics is Here](https://medium.com/celoorg/optics-is-here-42aa610675ce)  

- 2022-01-XX: [Nomad - a new design for radically cheaper cross-chain communication without header verification](https://docs.nomad.xyz/)  

- 2022-04-22: [Bridging Sapling: Private Cross-Chain Transfers](https://arxiv.org/abs/2204.10611)

## Federated pegs

- 2015-06-08: [Announcing Sidechain Elements: Open source code and developer sidechains for advancing Bitcoin](https://blockstream.com/2015/06/08/en-714/)  

- 2017-01-06: [Strong Federations: An Interoperable Blockchain Solution to Centralized Third Party Risks](https://blockstream.com/strong-federations.pdf)  

- 2019-01-29: [RSK: Bitcoin Powered Smart Contracts](https://www.rsk.co/Whitepapers/RSK-White-Paper-Updated.pdf)  

- 2020-05-22: [Liquid: A Bitcoin Sidechain](https://blockstream.com/assets/downloads/pdf/liquid-whitepaper.pdf)  

- 2020-12-02: [Building the Most Secure, Permissionless and Uncensorable Bitcoin Peg](https://medium.com/iovlabs-innovation-stories/building-the-most-secure-permissionless-and-uncensorable-bitcoin-peg-b5dc7020e5ec)  

- 2021-01-XX: [Minpeg, a miners' multisig in the peg](https://github.com/rsksmart/RSKIPs/blob/master/IPs/RSKIP198.md)  

## One-way pegs

- 2020-01-01: [Permissionless Bitcoin Childchains w/ Continuous Proof of Bitcoin Burn (CPoBB) and 2-way-value-pegs (2wvp)](https://bitcointalk.org/index.php?topic=5214173.0)  

- 2020-06-28: [Soft pegged sidechains](https://gist.github.com/fernandonm/cb9f719b125d93fb84e0988917bdde2a)  

- 2020-12-12: [Spacechains presentation](https://twitter.com/SomsenRuben/status/1337863852202090505)  

## Cross-chain atomic swaps

- 2018-06-23: [COMIT Network: Connect all the Blockchains!!!](https://comit.network/blog/2018/06/23/connect-all-the-blockchains)

- 2018-10-03: [Interledger: How to Interconnect All Blockchains and Value Networks](https://medium.com/xpring/interledger-how-to-interconnect-all-blockchains-and-value-networks-74f432e64543)  

- 2018-10-03: [The Missing Tool to Cross-Chain Development and Interoperable Blockchains: the Chain Abstraction Layer](https://medium.com/liquality/the-missing-tool-to-cross-chain-development-2ebfe898efa1)  

- 2020-05-11: [Succinct Atomic Swap](https://youtu.be/TlCxpdNScCA)  

- 2020-09-02: [Launching OpenDEX - The Decentralized Exchange Standard](https://blog.exchangeunion.com/launching-opendex-the-decentralized-exchange-standard-b907d2a99b5a)  

- 2021-01-12: [Vector 0.1.0 Mainnet Release](https://medium.com/connext/vector-0-1-0-mainnet-release-9496ae52c422)  

## Miscellaneous

- 2018-07-24: [Proposals to bridge to Ethereum](https://github.com/jpitts/eth-community-discussions/blob/master/proposals-to-bridge.md)  

- 2019-03-22: [Sidechains and interoperability](https://arxiv.org/pdf/1903.04077.pdf)  

- 2019-05-21: [Interchain Standards](https://github.com/cosmos/ics)  

- 2019-10-02: [SoK: Communication Across Distributed Ledgers](https://eprint.iacr.org/2019/1128.pdf)  

- 2020-01-12: [Coins: A Billion Bitcoin Users](https://coins.github.io/research/coins.pdf)  

- 2020-01-21: [Introducing Cross-Chain Group](https://medium.com/cross-chain-group/introducing-cross-chain-group-c9238e62509e)  

- 2021-01-28: [Hop: Send Tokens Across Rollups](https://hop.exchange/whitepaper.pdf)  

- 2021-08-05: [Introducing the Cross-Chain Interoperability Protocol (CCIP) for Decentralized Inter-Chain Messaging and Token Movements](https://blog.chain.link/introducing-the-cross-chain-interoperability-protocol-ccip/)  

- 2021-09-08: [Blockchain Bridges: Building Networks of Cryptonetworks](https://medium.com/1kxnetwork/blockchain-bridges-5db6afac44f8)  

- 2021-09-10: [The tradeoffs of cross-chain communication](https://ls.mirror.xyz/5FM0KUurAEkN7yDXLAI8i9kCha_yMlzguVqiHEGMjPU)  

- 2021-10-01: [The Interoperability Trilemma](https://medium.com/connext/the-interoperability-trilemma-657c2cf69f17)  

- 2021-10-04: [Clusters: how trusted & trust-minimized bridges shape the multi-chain landscape](https://blog.celestia.org/clusters/)

- 2021-10-25: [Across Protocol: Instant Trustless Token Transfers from Roll-up to Mainnet](https://drive.google.com/file/d/1t9tJUjJupLSvHKR8glwLKh8kpBNp5sp1/view)

- 2021-10-26: [Stakechain: A Bitcoin-backed Proof-of-Stake](https://raw.githubusercontent.com/coins/research/master/Bitcoin_backed_Proof_of_Stake.pdf)  

- 2022-01-20: [Babylon: Reusing Bitcoin Mining to Enhance Proof-of-Stake Security](https://eprint.iacr.org/2022/076)

# Bonus

- 2016-03-07: [My Sofa is a Sidechain](https://www.ic.unicamp.br/~stolfi/EXPORT/projects/bitcoin/posts/2015-06-10-my-sofa-is-a-sidechain/main.html)  
