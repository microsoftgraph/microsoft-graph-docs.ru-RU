---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cfbb92d872f49c57e2c4dc280db8708efafc005d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788324"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let policies = await client.api('/identity/conditionalAccess/policies')
    .get();

```