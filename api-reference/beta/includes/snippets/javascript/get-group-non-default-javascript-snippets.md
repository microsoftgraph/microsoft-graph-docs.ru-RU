---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 96c7d033f18c8f442b643316f97db56295551149
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785862"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd')
    .version('beta')
    .select('allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount')
    .get();

```