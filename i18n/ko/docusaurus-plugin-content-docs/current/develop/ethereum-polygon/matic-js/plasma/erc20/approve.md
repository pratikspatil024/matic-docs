---
id: approve
title: 승인
keywords:
  - 'pos client, erc20, approve, polygon, sdk'
description: 'maticjs 시작하기'
---

`approve` 메소드는 루트 토큰에 필요한 수량을 승인하는 데 사용될 수 있습니다.

폴리곤 체인에 금액을 입금하려면 승인이 필요합니다.

```
const erc20RootToken = plasmaClient.erc20(<root token address>, true);

// approve 100 amount
const approveResult = await erc20Token.approve(100);

const txHash = await approveResult.getTransactionHash();

const txReceipt = await approveResult.getReceipt();

```
