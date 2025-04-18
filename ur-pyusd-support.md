# PayPal USD stablecoin support in the Ur uncensorable application store

While this task seemed quite easy it has been actually kinda tricky.

The main reason is Google RPC service is mostly available
on Ethereum, a network which at the time of writing is hardly feasible
to be used for an application store.

Since uncensorability and permissionlessness are certainly Ur properties
I can't compromise on, without requiring users to bridge the token on cheaper networks
such as those on which the
[Ur](
  https://github.com/themartiancompany/ur)
is already deployed, it has seemed to me a
[one-way cross chain permissionless router bridge](
  https://github.com/themartiancompany/one-way-cross-chain-permissionless-router-bridge),
if implemented, could have been an acceptable constraints relaxation on permissionlessness.
Still though, there has not been time to complete that as well.

Most of the work during the past weeks has been focused on releasing
a stable version of the on-chain, network-neutral, uncensorable
[EVM Contracts Source Index](
  https://github.com/themartiancompany/evm-contracts-source-index),
in order to have users be sure of what's happening when they
purchase an application using a token they may be unfamiliar with
requiring them to execute its public `approve` and `transferFrom`
ERC-20 functions.

The task per-se has been
[completed in time](
  https://gnosisscan.io/tx/0x4981a14c955c18c8420245f74992e5342886d30674fa0e1566835c6cbdfde796),
and the kirsh application available
for purchase on the new Ur contract with the PYUSD token is
the decentralized Twitter.

The Ur video presentation is still a work in progress as the project
is quite complex and it is the fruit of an almost year-long work,
so it will probably be published on the 16th of April on X and
linked on this repository.
