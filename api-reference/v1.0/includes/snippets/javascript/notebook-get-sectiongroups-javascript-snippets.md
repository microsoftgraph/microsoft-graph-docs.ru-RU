---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6d00a1063df5ec45143c639d168a28c86887b35c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789687"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sectionGroups = await client.api('/me/onenote/notebooks/{id}/sectionGroups')
    .get();

```