---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2e2240c28eef4ac3b5bf8e2472df062925df3390
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795682"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/')
    .version('beta')
    .expand('extensions($filter=id%20eq%20\'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral\')')
    .get();

```