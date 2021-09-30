# Changelog

## UNRELEASED

### Bug Fixes

- [cronos#109](https://github.com/crypto-org-chain/cronos/issues/109) ibc transfer timeout too short
- [tharsis#590](https://github.com/tharsis/ethermint/pull/590) fix export contract state in genesis and reimport

### Features

- [cronos#110](https://github.com/crypto-org-chain/cronos/pull/110) embed swagger doc ui
- [cronos#113](https://github.com/crypto-org-chain/cronos/pull/113) export token mapping state to genesis

*September 22, 2021*
## v0.5.4

This version is the same as v0.5.3 with a patched version of ethermint which include a bug fix on the transaction receipts events and on concurrent query.

### Bug Fixes

- [cronos#93](https://github.com/crypto-org-chain/cronos/pull/93) tx receipts don't contain events
- [cronos#98](https://github.com/crypto-org-chain/cronos/pull/98) node crash under concurrent query

*September 21, 2021*
## v0.5.3

This version contains several new features, it enables gravity bridge in Cronos and automatic token conversion for bridging tokens to crc20 tokens. It also fix the decimal conversion issues in the CRO tokens from crypto.org chain.
In addition to that, it also upgrade ethermint to its latest version (v0.5.0.x) which bring several breaking changes (see [changelog](https://github.com/tharsis/ethermint/blob/1a01c6a992c0fb94d70bb1c7127715874cefd057/CHANGELOG.md)).

### Consensus breaking changes
- [cronos#87](https://github.com/crypto-org-chain/cronos/pull/87) upgrade ethermint to v0.4.2-0.20210920104419-1a01c6a992c0

### Features

- [cronos#11](https://github.com/crypto-org-chain/cronos/pull/11) embed gravity bridge module
- [cronos#35](https://github.com/crypto-org-chain/cronos/pull/35) add support for ibc hook
- [cronos#55](https://github.com/crypto-org-chain/cronos/pull/55) add support for ibc token conversion to crc20
- [cronos#45](https://github.com/crypto-org-chain/cronos/pull/45) allow evm contract to call bank send and gravity send
- [cronos#65](https://github.com/crypto-org-chain/cronos/pull/65) support SendToIbc in evm_log_handlers
- [cronos#59](https://github.com/crypto-org-chain/cronos/pull/59) gravity bridged tokens are converted to crc20
  automatically
- [cronos#68](https://github.com/crypto-org-chain/cronos/issues/68) support SendCroToIbc in evm_log_handlers
- [cronos#86](https://github.com/crypto-org-chain/cronos/issues/86) change account prefix

*August 19, 2021*

## v0.5.2

### Consensus breaking changes

- (ethermint) [tharsis#447](https://github.com/tharsis/ethermint/pull/447) update `chain-id` format.

### Improvements

- (ethermint) [tharsis#434](https://github.com/tharsis/ethermint/pull/434) configurable vm tracer

### Bug Fixes

- (ethermint) [tharsis#446](https://github.com/tharsis/ethermint/pull/446) fix chain state export issue



*August 16, 2021*

## v0.5.1

This version is a new scaffolding of cronos project where ethermint is included as a library.

### Consensus breaking changes

- (ethermint) [tharsis#399](https://github.com/tharsis/ethermint/pull/399) Exception in sub-message call reverts the call if it's not propagated.
- (ethermint) [tharsis#334](https://github.com/tharsis/ethermint/pull/334) Log index changed to the index in block rather than tx.
- (ethermint) [tharsis#342](https://github.com/tharsis/ethermint/issues/342) Don't clear balance when resetting the account.
- (ethermint) [tharsis#383](https://github.com/tharsis/ethermint/pull/383) `GetCommittedState` use the original context.

### Features

### Improvements

- (ethermint) [tharsis#425](https://github.com/tharsis/ethermint/pull/425) Support build on linux arm64
- (ethermint) [tharsis#423](https://github.com/tharsis/ethermint/pull/423) Bump to cosmos-sdk 0.43.0

### Bug Fixes

- (ethermint) [tharsis#428](https://github.com/tharsis/ethermint/pull/428) [tharsis#375](https://github.com/tharsis/ethermint/pull/375) Multiple web3 rpc api fixes.