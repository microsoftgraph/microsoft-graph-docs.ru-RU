---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3aa63c563be2f20374fd3487e5a227e513ecabc6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791720"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const threatAssessmentRequest = {
  '@odata.type': '#microsoft.graph.urlAssessmentRequest',
  url: 'http://test.com',
  expectedAssessment: 'block',
  category: 'phishing'
};

await client.api('/informationProtection/threatAssessmentRequests')
    .post(threatAssessmentRequest);

```