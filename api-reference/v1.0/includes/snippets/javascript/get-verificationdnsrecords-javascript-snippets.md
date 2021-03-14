---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6cb0c7572c539e84af4c1368060f102fb6c47d0b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784012"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let verificationDnsRecords = await client.api('/domains/{domain-name}/verificationDnsRecords')
    .get();

```