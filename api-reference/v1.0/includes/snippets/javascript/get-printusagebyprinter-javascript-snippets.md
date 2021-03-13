---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dc7bd7a6a73576650ee1dfd8154f8f6a9d5d2e29
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774470"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printUsageByPrinter = await client.api('/reports/dailyPrintUsageByPrinter/{id}')
    .get();

```