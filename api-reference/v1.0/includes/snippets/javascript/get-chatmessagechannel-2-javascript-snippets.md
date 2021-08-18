---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 04d25e62aad9447771ffab6a17caac1775a709cc806c6272ff9256ab0d991bc5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57428311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chatMessage = await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1614618259349')
    .get();

```