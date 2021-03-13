---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dc0404423105284dcce1cebc577ead952e4fb0a9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799570"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let hostedContents = await client.api('/chats/{id}/messages/{id}/hostedContents')
    .version('beta')
    .get();

```