---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 18e10049cc8f73b1a05a690b2fa3d83270701a22
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804298"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissions = await client.api('/me/drive/items/{item-id}/permissions')
    .get();

```