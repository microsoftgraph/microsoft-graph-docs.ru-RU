---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f0c6c7e17a3c4f5abd4ad760fab5696054dc9b32
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803541"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let businessFlowTemplates = await client.api('/businessFlowTemplates')
    .version('beta')
    .get();

```