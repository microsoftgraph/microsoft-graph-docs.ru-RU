---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eb07d678bad85dccaad3d56434ccc37c61390668
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787180"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/chats/{id}/members')
    .get();

```