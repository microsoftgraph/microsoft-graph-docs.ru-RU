---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a66960065fe03fb41835e0e30dcfda1e83a54cb0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792854"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channel = await client.api('/teams/{id}/primaryChannel')
    .version('beta')
    .get();

```