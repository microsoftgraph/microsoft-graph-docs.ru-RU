---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ce6c203fa066b480c5319ad077f53a2d5d9b6f30
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2020
ms.locfileid: "40871925"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/informationProtection/threatAssessmentRequests')
    .version('beta')
    .get();

```