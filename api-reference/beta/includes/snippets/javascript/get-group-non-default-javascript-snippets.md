---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2cb0902929faacd24732ff16d0c81f2850bcd7ae48095b07af09819593f43db5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57363055"
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