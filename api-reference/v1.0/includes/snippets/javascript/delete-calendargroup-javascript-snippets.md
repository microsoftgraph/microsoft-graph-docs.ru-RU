---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1e114334b9f1cab21b283eea54f605e410f5ece6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809323"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/calendarGroups/{id}')
    .delete();

```