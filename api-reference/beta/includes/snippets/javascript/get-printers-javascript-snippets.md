---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 344c4a11826dbfe7f90bdfe77fcbf13dd0cc83e7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782905"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printers = await client.api('/print/printers')
    .version('beta')
    .get();

```