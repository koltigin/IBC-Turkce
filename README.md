# IBC

![banner](./assets/interchain-standards-image.jpg)

## Sinopsis

Bu depo, blok zincirler arası iletişim protokolünün (IBC) geliştirilmesi ve belgelenmesi için bir standarttır.

Hem çekirdek aktarım, kimlik doğrulama ve sipariş katmanı (IBC/TAO) hem de paket kodlama ve işleme anlambilimini (IBC/APP) açıklayan uygulama katmanları dahil olmak üzere, tasarım mantığı, protokol semantiği ve IBC için kodlama açıklamalarını birleştirmek için kullanılacaktır.

Katkılar memnuniyetle karşılanmaktadır. Katkı yönergeleri için [CONTRIBUTING.md](meta/CONTRIBUTING.md) bölümüne bakınız.

Yol haritamızın herkese açık güncel sürümü için [ROADMAP.md](meta/ROADMAP.md) adresine bakınız.

## IBC Nedir?

IBC'nin ne olduğuna ve nasıl çalıştığına ilişkin ayrıntılı bir açıklama için lütfen [bu blog gönderisini](https://blog.cosmos.network/eli5-what-is-ibc-a212f518715f) okuyunuz.

## Zincirler Arası Standartlar (Interchain Standards)

"Taslak" aşamasındaki veya bundan sonraki tüm standartlar, kategoriye göre sıralanmış ICS numaralarına göre burada listelenir.

### Meta

| Zincirler Arası Standart Numarası               | Standart Başlığı             | Aşama |
| ---------------------------------------- | -------------------------- | ----- |
| [1](spec/ics-001-ics-standard/README.md) | ICS Specification Standard | N/A   |

### Core

| Zincirler Arası Standart Numarası                             | Standart Başlığı           | Aşama     | Uygulamalar |
| ------------------------------------------------------------- | -------------------------- | --------- | --------------- |
| [2](spec/core/ics-002-client-semantics/README.md)             | Client Semantics           | Candidate | [ibc-go](https://github.com/cosmos/ibc-go) |
| [3](spec/core/ics-003-connection-semantics/README.md)         | Connection Semantics       | Candidate | [ibc-go](https://github.com/cosmos/ibc-go) |
| [4](spec/core/ics-004-channel-and-packet-semantics/README.md) | Channel & Packet Semantics | Candidate | [ibc-go](https://github.com/cosmos/ibc-go) |
| [5](spec/core/ics-005-port-allocation/README.md)              | Port Allocation            | Candidate | [ibc-go](https://github.com/cosmos/ibc-go) |
| [23](spec/core/ics-023-vector-commitments/README.md)          | Vector Commitments         | Candidate | [ibc-go](https://github.com/cosmos/ibc-go) |
| [24](spec/core/ics-024-host-requirements/README.md)           | Host Requirements          | Candidate | [ibc-go](https://github.com/cosmos/ibc-go) |
| [25](spec/core/ics-025-handler-interface/README.md)           | Handler Interface          | Candidate | [ibc-go](https://github.com/cosmos/ibc-go) |
| [26](spec/core/ics-026-routing-module/README.md)              | Routing Module             | Candidate | [ibc-go](https://github.com/cosmos/ibc-go) |

### Client

| Zincirler Arası Standart Numarası                               | Standart Başlığı           | Aşama | Uygulamalar |
| --------------------------------------------------------------- | -------------------------- | ----- | --------------- |
| [6](spec/client/ics-006-solo-machine-client/README.md)          | Solo Machine Client        | Candidate | [ibc-go](https://github.com/cosmos/ibc-go/tree/main/modules/light-clients/06-solomachine) |
| [7](spec/client/ics-007-tendermint-client/README.md)            | Tendermint Client          | Candidate | [ibc-go](https://github.com/cosmos/ibc-go/tree/main/modules/light-clients/07-tendermint) |
| [8](spec/client/ics-008-wasm-client/README.md)                  | Wasm Client                | Draft | |
| [9](spec/client/ics-009-loopback-client/README.md)              | Loopback Client            | Draft | |
| [10](spec/client/ics-010-grandpa-client/README.md)              | GRANDPA Client             | Draft | |

### Relayer

| Zincirler Arası Standart Numarası                                | Standart Başlığı           | Aşama | Uygulamalar |
| ---------------------------------------------------------------- | -------------------------- | ----- | --------------- |
| [18](spec/relayer/ics-018-relayer-algorithms/README.md)          | Relayer Algorithms         | Finalised | [go-relayer](https://github.com/cosmos/relayer), [rust-relayer](https://github.com/informalsystems/ibc-rs), [ts-relayer](https://github.com/confio/ts-relayer) |

### App

| Zincirler Arası Standart Numarası                        | Standart Başlığı        | Aşama | Uygulamalar |
| -------------------------------------------------------- | ----------------------- | ----- | --------------- |
| [20](spec/app/ics-020-fungible-token-transfer/README.md) | Fungible Token Transfer | Candidate | [ibc-go](https://github.com/cosmos/ibc-go/tree/main/modules/apps/transfer) |
| [27](spec/app/ics-027-interchain-accounts/README.md)     | Interchain Accounts     | Candidate | [ibc-go](https://github.com/cosmos/ibc-go/tree/main/modules/apps/27-interchain-accounts) |
| [28](spec/app/ics-028-cross-chain-validation/README.md)  | Cross-Chain Validation  | Draft | |
| [29](spec/app/ics-029-fee-payment) | General Relayer Incentivisation Mechanism | Candidate | [ibc-go](https://github.com/cosmos/ibc-go/tree/main/modules/apps/29-fee) |
| [30](spec/app/ics-030-middleware) | IBC Application Middleware | N/A | N/A |
| [31](spec/app/ics-031-crosschain-queries) | Cross-Chain Queries | Draft | N/A |
| [721](spec/app/ics-721-nft-transfer) | Non-Fungible Token Transfer | Candidate | [bianjieai](https://github.com/bianjieai/ibc-go/tree/ics-721-nft-transfer) |
