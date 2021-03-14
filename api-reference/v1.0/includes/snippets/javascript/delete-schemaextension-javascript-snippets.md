---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c5938394365b334d6253fc2b41591c9ff7bab909
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800456"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/schemaExtensions/{id}')
    .delete();

```