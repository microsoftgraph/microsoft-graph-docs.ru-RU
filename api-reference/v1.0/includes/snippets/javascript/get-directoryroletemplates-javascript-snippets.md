---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ca94fbcb893ab014c8574535cda79d2ef9b35ff3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779370"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRoleTemplates = await client.api('/directoryRoleTemplates')
    .get();

```