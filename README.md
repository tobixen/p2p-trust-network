# p2p-trust-network

This is so far just some loose ideas

## Rationale

Often it's useful to be able to trust an online identity, i.e. for peer-to-peer lending sites, peer-to-peer home exchange sites, work assignments, etc.

Most often the various platforms (like Couchsurfing, Uber, BeWelcome, Loanbase, Localbitcoins etc) will have some built-in support for ratings; user account A can leaving positive feedback for B after A and B has had an interaction on that platform.  The ratings never leave the platform.  There are usually no ways to see the difference between a conman creating yet another fake account and a newcomer to the platform.  It is impossible for an outsider that have been scammed on one platform to leave a negative feedback warning users on another platform about the scammer.

What we need is a global network-of-trust system.  It should be truely peer-to-peer, it should be based on open standards and open source.  Just the risk of getting negative feedback on such a network could be enough deterrent to avoid certain types of scam.

## Features needed

A real person should be able to record personal details.

A real person should be able to record various online identities and link them up to the personal details.

A real person should be able to record different kind of trust in the system, like "I've met Peter and verified his ID documents", "I know the real person Peter has the username peter123 on Google Buzz", "Peter cannot be trusted", "I borrowed my car to Peter and he never came back with it", "I endorse Peter for his knowledge of greek ancient history", etc.

One should be able to query an online identity and if there is any kind of chain between you and this account it should be visible.

It should be easy to import/sync data from existing systems.  I.e, importing data from PGP "web-of-trust", importing data from sites like LinkedIn and Facebook, etc.

## Privacy and problems

Such a network will contain a lot of valuable metadata that can be abused in all sorts of ways - that's something to be concerned over.  One should consider smart ways to use encryption.

Such a network is also quite open to unjust revenge-attacks from angry ex-partners, etc.

## Implementation details

A global database - perhaps something blockchain-based?

## Existing works

* OpenPGP key signings is already some form of "web-of-trust"-network - but it has quite some weaknesses, it is only useful for connecting email addresses with real names.  A keysigning supposedly should be read as "I have checked the ID documents of Eve", though it's normal to skip the ID verification process.
* PeerTrust - http://www.cc.gatech.edu/projects/disl/PeerTrust/ - seems to be a white paper from 2004.  The "Related Work"-section contains only dead links
* Keybase - keybase.io
* Namecoin
* Orisi
* Onename
