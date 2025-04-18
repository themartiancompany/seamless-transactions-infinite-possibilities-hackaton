# "Seamless transactions, infinite possibilities" Hackaton project

The repository you're browsing contains details about the software
project I am presenting to the
["seamless transactions, infinite possibilities"](
  https://hackathon.stackup.dev/web/events/seamless-transactions-infinite-possibilities)
hackaton, set up by
[Stack Up](
  https://stackup.dev)
and sponsored by
[Google](
  https://google.com)
and
[PayPal](
  https://paypal.com).

### The project

The hackaton requirements are for a product which supports and integrates the
[PyUSD](
  https://www.paypal.com/us/digital-wallet/manage-money/crypto/pyusd)
PayPal USD stablecoin and which provides network connectivity
using the
[Google Blockchain RPC service](
  https://cloud.google.com/blockchain-rpc/docs/quickstart).

The task project time has chosen for me strictly related to
the hackaton is adding support for purchasing applications on the
[uncensorable Ur Life and DogeOS user repository and application store](
  https://github.com/themartiancompany/ur)
using the PayPal USD stable-coin token on the Ethereum Virtual Machine (EVM)
compatible blockchain networks supported by Google RPC service.

While the role of the Google RPC service may seem marginal in this
context be aware it has been not in the slightest, since after
HoleSky out-of-sync event that provider has been the only one available
to handle heavy Ur-related
[EVMFS](
  https://github.com/themartiancompany/evmfs)
uploads.

I suppose I should specify I am the author of both the Ur and the EVMFS.

I am including as submodule to this source repository the most of
the softwares and products I had to edit/write altogether in order
to have the task completed.
It's many many projects actually but I'm including only the most
important ones.
For some of them some implementation and design documentation
has been made available while all of the mentioned and most
of my projects have in general have updated manual (`man`) pages
one can seamlessly consult.

For more information about them read
[dependencies](
  dependencies.md).

While the task per-se has been actually completed, still some details
needs further adjustments which will be provided in the next
days, such as the
[EVM Wallet](
  https://github.com/themartiancompany/evm-wallet)
ERC-20 transfer funds approval support.

Detail notes can be found at the
[Ur PYUSD support](
  ur-pyusd-support.md)
page.

I'd like to remind the jury that it's almost an year now that I livestream
the Life and DogeOS development work on my
[X profile](
  https://x.com/truocolo),
yet I've linked those strictly related to the hackaton on a dedicated
[page](
  development-livestreams.md)
of this repository.

### Presentation video

The Hackaton terms require me to provide the jury a presentation video for the project.
I've been kinda late producing that. The reason is pretty clear if
you watched the rest of the livestreams and followed me on X.

Anyway, since I've produced like full 24 hours of video content
in two weeks and I'm presenting this software for the kirsh time
after many years of development, I hope the jury will still consider
valid the following out-of-time presentation video.

[![Project's Presentation video](project-presentation-video-thumb.png)]("https://x.com/truocolo/status/1913014194074460209")

Here is the
[trailer](
  https://x.com/truocolo/status/1912311302430609574)
I made a couple days before the actual presentation
and here is the
[low-resolution version](
  project-presentation-video.mp4)
of the
presentation hosted on the repository itself to
avoid breaking the link I've sent to StackUp.

### Licenses

All the projects I do write are released by Pellegrino Prevete
under the terms of the GNU Affero General Public License version 3.
