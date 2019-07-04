---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a66f8f0fe7e8fc194c06cef65a0669bb2a45b617
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35515963"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const domain = {
  isDefault: true,
  supportedServices: [
    "Email",
    "OfficeCommunicationsOnline"
  ]
};

let res = await client.api('/domains/contoso.com')
    .update({domain : domain});

```