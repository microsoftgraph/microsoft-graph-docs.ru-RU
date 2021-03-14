---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 133d80ac241c2c26621fe423a92acbf9d0d65225
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798831"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contactFolder = await client.api('/me/contactFolders/{id}')
    .get();

```