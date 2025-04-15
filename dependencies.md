# Dependencies

On this page I group and shortly discuss some of
the direct or indirect software dependencies
I had to write in order to complete the main
task and of which I am the main or the only author.

### [Crash Bash](https://github.com/themartiancompany/crash-bash)

I've written this application development Bash library a couple years
ago and I still use it as of today in most of them.

The exported functions and the way they are called from the programs
using them originally mimicked the original
ArchLinux's
[Archiso](
  https://github.com/themartiancompany/archiso),
which I've worked on for the same amount of time before
eventually taking over the project altogether for lack
of review activity from the rest of the team members
and their little consideration for some very basic
physical security vulnerabilities and features the
artifacts the program generates was respectively
subject to and which had been readily and promptly
made available.

### [LibEVM](https://github.com/themartiancompany/libevm)

The EVM Library contains a set of useful functions to
write native computer applications interacting with
EVM blockchain networks.

### [Aspe](https://github.com/themartiancompany/aspe)

Aspe is Ur reference source recipe retrieval tool.

### [Pub](https://github.com/themartiancompany/pub)

Pub is Ur reference source recipe publishing tool.

I have preferred to have both Aspe and Pub standalone
rather than integrating them directly into the Ur
so to encourage alternative implementations as
well as having them support different protocol
backends.

### [Ethereum Virtual Machine GNU Privacy Guard](https://github.com/themartiancompany/evm-gnupg)

The EVM GNUPG is a Bash GNUPG wrapper dedicated to manage
GNUPG EVM's external owner account (*EOA*) identities.

### [Ethereum Virtual Machine OpenPGP Key Server](https://github.com/themartiancompany/evm-openpgp-keyserver)

The EVM OpenPGP Key Server is an on-chain, network-independent,
uncensorable, permissionless OpenPGP Key Server.

### [Ethereum Virtual Machine File System](https://github.com/themartiancompany/evmfs)

The EVMFS is the uncensorable, undeletable file system for EVM networks
I've written in order to safely manage almost any kind of online
binary resources.
It is extensively used in all the applications reported in this page.

### [Ethereum Virtual Machine Contracts' Source Index](https://github.com/themartiancompany/evm-contracts-source-index)

The EVM Contracts' Source Index is an on-chain, undeletable, uncensorable,
network-independent, network-neutral, permissionless EVM deployed contracts'
Source code Index.

It resolves the decade long issue of Ethereum developers not having provided
users with a facility to host contracts' source code on-chain directly,
so forcing them to rely on third party, centralized, network-specific
blockchain network explorers.

### [Ethereum Virtual Machine Contracts' Tools](https://github.com/themartiancompany/evm-contracts-tools)

### [Ethereum Virtual Machine Transactions' Tools](https://github.com/themartiancompany/evm-transactions-tools)

