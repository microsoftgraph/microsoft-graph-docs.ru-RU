---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 272682e9f32f8ec8b8f6cb88c8cfc416a484dc7d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801809"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getCredentialUsageSummary = await client.api('/reports/getCredentialUsageSummary(period='D30')')
    .version('beta')
    .filter('feature eq \'registration\'')
    .get();

```