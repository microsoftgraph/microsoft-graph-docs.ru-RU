---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: add7e8addc6d9a3e436914a94ba39f9351d52048
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778650"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applicationTemplate = await client.api('/applicationTemplates/{id}')
    .version('beta')
    .get();

```