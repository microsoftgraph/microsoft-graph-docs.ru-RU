---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 29263615e48687f976dc0d2d05544e23081b27d1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778788"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schemaExtension = await client.api('/schemaExtensions/graphlearn_test')
    .version('beta')
    .get();

```