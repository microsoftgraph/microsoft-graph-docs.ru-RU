---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f5f599e3a562de7a08f92ca8e2d0a0c6d246a83c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782134"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/schools/{school-id}/classes/{class-id}')
    .delete();

```