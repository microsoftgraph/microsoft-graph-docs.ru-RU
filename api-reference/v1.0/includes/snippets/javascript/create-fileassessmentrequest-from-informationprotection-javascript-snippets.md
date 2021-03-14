---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5ae4cdc5b49a2424875eaedea5ce70839ebb6a1b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797183"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const threatAssessmentRequest = {
  '@odata.type': '#microsoft.graph.fileAssessmentRequest',
  expectedAssessment: 'block',
  category: 'malware',
  fileName: 'test.txt',
  contentData: 'VGhpcyBpcyBhIHRlc3QgZmlsZQ=='
};

await client.api('/informationProtection/threatAssessmentRequests')
    .post(threatAssessmentRequest);

```