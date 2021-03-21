---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dc6c924c3a4fc4ce28a80b20f22c5d3fe7c559a2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954828"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let dailyPrintUsageByUser = await client.api('/reports/dailyPrintUsageByUser')
    .get();

```