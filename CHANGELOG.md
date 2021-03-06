# Changelog

## 0.12.1 (Jul 20, 2018)

* Add `timeout` and `attempts` parameters to the `send` method. #116

## 0.11.1 (Jul 10, 2018)

* Updated explorer API. #114
New web API based on `actix-web` implemented in Exonum core [0.9][release-0.9].

## 0.11.0 (Jul 9, 2018)

* Remove field `schema_version` from `Block` structure. #115
Field is removed in Exonum core [0.9][release-0.9].

## 0.10.2 (Jun 29, 2018)

* Rework version import to fix library babelify using webpack. #112

## 0.10.1 (Jun 25, 2018)

* Fix serialization of custom data types of 2 and more nesting level. #110

## 0.10.0 (Jun 20, 2018)

* Add serialization support of decimal type (`Decimal`). #108
Decimal type is added into Exonum core in [0.8][release-0.8].

## 0.9.0 (Jun 18, 2018)

* Add support of `UUID` serialization. #97

## 0.8.2 (May 23, 2018)

* Refactor `send` method to remove dependency onto service response format during pushing the transaction. #103

## 0.8.1 (May 21, 2018)

* Add a new `version` property to check library version. #101
* Cover the case when the blockchain explorer down or return the unexpected response. #102

## 0.8.0 (May 15, 2018)

* Add a new `send` method to send transaction to the blockchain. #98
* Add a new `sendQueue` method to send multiple transactions to the blockchain. #98

## 0.7.3 (Apr 30, 2018)

* Update third-party dependencies to fix potential security vulnerabilities. #96

## 0.7.2 (Apr 11, 2018)

* Add static `hash` method to `Exonum.Hash` primitive type. #94

## 0.7.1 (Apr 11, 2018)

* Fix missed `MapProof` method. #93

## 0.7.0 (Apr 11, 2018)

* Proofs of existence in Merkle Patricia tree have been replaced with Map proof. #85
Method is replaced in Exonum core in [0.7][release-0.7].
* `network_id` attribute has been removed from custom data types, transactions and proofs. #90
Attribute is removed in Exonum core in [0.7][release-0.7].

## 0.6.1 (Apr 4, 2018)

* Add Uint8Array to Binary String convertor (`uint8ArrayToBinaryString` method). #88

## 0.6.0 (Mar 24, 2018)

* Custom data type and transaction no longer require manual `size`, `from` and `to` specification.
This feature is added into Exonum core in [0.5][release-0.5]. #84

## 0.5.0 (Mar 6, 2018)

* Add serialization support of floating point types (`Float32` and `Float64`). #83
Floating point types are added into Exonum core in [0.5][release-0.5].
* Add [package-lock.json](package-lock.json). #81

## 0.4.1 (Feb 23, 2018)

* Fix issue with converting of Binary String to Uint8Array (`binaryStringToUint8Array` method).
This problem also affected the validation of the Merkle Patricia tree. #80

## 0.4.0 (Feb 9, 2018)

* Change order of bytes and bits in the `DBKey` keys of Merkle Patricia. #78
Order is changed in Exonum core in [0.5][release-0.5].
* Extend usage examples and move them into separate files. #77
* Improve tests readability. #75 #76

## 0.3.0 (Nov 20, 2017)

* Remove `FixedBuffer` type because it is not supported by core by default. #71

## 0.2.3 (Sep 27, 2017)

* Fix issue with serialization of transactions. #70

## 0.2.2 (Sep 26, 2017)

* Fix issue with serialization of transactions. #69

## 0.2.1 (Sep 20, 2017)

* Add serialization support of array type (`newArray`). #63
* Change the way of `Array` and `String` serialization. #58
* Use `standard` lint rules. #64 #65

## 0.2.0 (Aug 1, 2017)

* Fix issue with Merkle Patricia Tree processing (`merklePatriciaProof` method). #53

## 0.1.1 (Jul 21, 2017)

* Add automatic publishing of new releases into npm via Travis CI. #54

## 0.1.0 (Jul 18, 2017)

The first release of JavaScript client for Exonum blockchain,
matching [release 0.1][release-0.1] of the Exonum core repository.

[release-0.9]: https://github.com/exonum/exonum/blob/master/CHANGELOG.md#090---2018-07-19
[release-0.8]: https://github.com/exonum/exonum/blob/master/CHANGELOG.md#08---2018-05-31
[release-0.7]: https://github.com/exonum/exonum/blob/master/CHANGELOG.md#07---2018-04-11
[release-0.5]: https://github.com/exonum/exonum/blob/master/CHANGELOG.md#05---2018-01-30
[release-0.1]: https://github.com/exonum/exonum/releases/tag/v0.1
