---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0ee961ab9ab5c98f8db9379a74a3020c1a1fdd73
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793787"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sites = await client.api('/sites?search=%7Bquery%7D')
    .get();

```