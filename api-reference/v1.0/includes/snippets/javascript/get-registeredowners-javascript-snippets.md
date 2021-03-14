---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5362a01b2ac0e1d97d980e1918c35269abe55bac
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799486"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let registeredOwners = await client.api('/devices/{id}/registeredOwners')
    .get();

```