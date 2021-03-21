---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fa003356006d66fa84bc2e8a89dd7f9300d3013f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954249"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let monthlyPrintUsageSummariesByUser = await client.api('/print/reports/monthlyPrintUsageSummariesByUser')
    .version('beta')
    .get();

```