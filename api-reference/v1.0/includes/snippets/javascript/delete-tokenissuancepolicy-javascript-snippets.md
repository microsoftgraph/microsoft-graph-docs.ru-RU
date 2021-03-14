---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 98650174cf6ecb1a779f9350c4d08958484a8fb6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789453"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/tokenIssuancePolicies/{id}')
    .delete();

```