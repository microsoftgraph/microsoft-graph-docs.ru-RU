---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c712baeafcd836041348443af296af9eca6a1061
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778100"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewScheduleDefinition = await client.api('/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d')
    .version('beta')
    .get();

```