---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a53fcab4068317d47823e0659f31a740d174f5c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797528"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectionOperation = await client.api('/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323')
    .version('beta')
    .get();

```