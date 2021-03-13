---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bd4464d4ae001a16b1ca989451cbf2171d157002
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797829"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationFlowsPolicy = await client.api('/policies/authenticationFlowsPolicy')
    .version('beta')
    .get();

```