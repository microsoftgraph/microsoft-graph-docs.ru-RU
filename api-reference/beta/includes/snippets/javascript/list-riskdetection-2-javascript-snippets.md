---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 98a84e281bb19f0ffa8b1ae3928aaddd32b78eac
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955565"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskDetection = await client.api('/identityProtection/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3')
    .version('beta')
    .get();

```