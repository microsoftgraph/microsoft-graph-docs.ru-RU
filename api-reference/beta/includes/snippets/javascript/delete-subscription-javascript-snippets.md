---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 78dd60340f8289f2098e519bb8047b68ed7eee72
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801106"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07')
    .version('beta')
    .delete();

```