---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 65b9c3ef509c41531b9ba6b0898e297e20bfeb3c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771941"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let shares = await client.api('/print/printers/{printerId}/shares')
    .get();

```