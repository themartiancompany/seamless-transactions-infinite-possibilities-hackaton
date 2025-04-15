# Dependencies

On this page I group and shortly discuss some of
the direct or indirect software dependencies
I had to write in order to complete the main
task and of which I am the main or the only author.

All together, these applications make
dapps development virtually the same as
the development of any other computer application.

## Run-time dependencies

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

### [Crash JavaScript](https://github.com/themartiancompany/crash-js)

Modeled after the Crash Bash library, it provides for JavaScript
programs the same utilities Crash Bash provides for Bash
programs.

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

I suppose it must be underlined the file system has its own dependency tree,
which seems to me large enough not to see fit for the scope of this page.

For further information about them consult the file system documentation.

### [Ethereum Virtual Machine Contracts' Source Index](https://github.com/themartiancompany/evm-contracts-source-index)

The EVM Contracts' Source Index is an on-chain, undeletable, uncensorable,
network-independent, network-neutral, permissionless EVM deployed contracts'
Source code Index.

It resolves the decade long issue of Ethereum developers not having provided
users with a facility to host contracts' source code on-chain directly,
so forcing them to rely on third party, centralized, network-specific
blockchain network explorers.

While apparently not a direct dependency, the Index is actually required
in order to properly present for manual verification the source code
for a novel currency token, for example the bridged PayPal stablecoin ERC-20,
encountered while purchasing an Ur application.

### [Ethereum Virtual Machine Contracts' Tools](https://github.com/themartiancompany/evm-contracts-tools)

Calls to `evm-contract-call` from the EVM Contracts' tools are used in
all libEVM applications which do not implement a dedicated JavaScript
program to communicate with the contract.

The caller program is able to automatically retrieve the target
contract source code, and so the needed contract artifacts from
the Source Index to run it.

While all libEVM programs such as the Ur should specify
a default system-level network deployment together with
the artifacts needed to run it, this feature is greatly
useful when testing a new or a new version for a contract.

Currently the Ur does not contain any application-specific JavaScript
program and all contract calls are handled by `evm-contract-call`.

### [Ethereum Virtual Machine Transactions' Tools](https://github.com/themartiancompany/evm-transactions-tools)

The EVM Transactions Tools are a dependency for the `evm-contract-deployer-get`
program from the EVM Contract Tools, which is used to validate the Index provided
deployent transaction in order to infer the contract deployer, whose
self-published sources are the default Index source download target.

### [Ethereum Virtual Machine Wallet](https://github.com/themartiancompany/evm-wallet)

All libEVM programs, in particular those requiring calls authentication,
import functions from the EVM Wallet libraries or call it directly.

## Build-time and development dependencies

### [Ethereum Virtual Machine Make](https://github.com/themartiancompany/evm-make)

The EVM Make program is a build dependency for
libEVM programs. While on single-networks deployments
contract artifacts and sources can be easily managed
manually, this tool becomes a necessity when a libEVM
application handles many smart contract versions
over many networks all at once.

### [Solidity Compiler](https://github.com/themartiancompany/solidity-compiler)

Solidity compiler is a unified front-end for Solc and Hardhat, aiming at
providing an user experience similar to the one of a C compiler.

### [Ethereum Virtual Machine Deployer](https://github.com/themartiancompany/evm-deployer)

While not strictly a dependency for any of the above program, an EVM Deployer
run on a solidity source file builds it, deploy it and publish it on the Index
in a single step, so greatly speeding up contract testing.
Together with the contract caller, it makes interacting with a contract deployment
not much different from interacting for example with a C binary saved
at an environment-specific location, in this case at the contract address.
