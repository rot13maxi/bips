<pre>
  BIP: ???
  Layer: Consensus (soft fork)
  Title: COVOPS: CAT + CHECKSIGFROMSTACK + OP_CHECKTEMPLATEVERIFY
  Author: Rijndael <rot13maxi@protonmail.com>
  Comments-URI: https://github.com/bitcoin/bips/wiki/Comments:BIP-????
  Status: Draft
  Type: Standards Track
  Created: 2024-12-12
  License: MIT
  Requires: 119, 347, 348
</pre>

## Abstract

This BIP describes a package of three opcodes for Tapscript: `OP_CAT`, `OP_CHECKSIGFROMSTACK`, and `OP_CHECKTEMPLATEVERIFY`. 
Together, these opcodes enable a variety of new Bitcoin Script constructions. Many of these constructions are applications of
covenants and delegation, so the package is called COVOPS, short for "Covenant Operations".

## Motivation


## Specification


## Rationale

## Backwards Compatibility

All three new opcodes add further constraints to OP_SUCCESS opcodes in Tapscript. Nodes that do not implement or enforce these opcodes
(either because they have not upgrades, or because they are running an alternative implementation that does not implement these opcodes) will
interpret any script that contains any of these opcodes as `TRUE`, meaning that this upgrade can be deployed as a soft fork.


## Reference Implementation

A reference implementation is provided in provided here:

https://github.com/bitcoin/bitcoin/pull/?????


## Deployment

TBD


## Copyright

This document is licensed under the MIT license.

[BIP 119]: https://github.com/bitcoin/bips/blob/master/bip-0119.mediawiki

[BIP 347]: https://github.com/bitcoin/bips/blob/master/bip-0347.mediawiki

[BIP 348]: https://github.com/bitcoin/bips/blob/master/bip-0348.mediawiki
