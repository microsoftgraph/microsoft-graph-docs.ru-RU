---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3ad4d3fe3bff76045511cd70846242863bfaa3bf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800474"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let projectParticipation = await client.api('/me/profile/projects/{id}')
    .version('beta')
    .get();

```