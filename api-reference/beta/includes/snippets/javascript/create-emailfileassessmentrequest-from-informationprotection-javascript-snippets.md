---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 68b9e94001ebe2dd62207b3dc5a542c065b9f1f2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784727"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const threatAssessmentRequest = {
  '@odata.type': '#microsoft.graph.emailFileAssessmentRequest',
  recipientEmail: 'tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com',
  expectedAssessment: 'block',
  category: 'malware',
  contentData: 'UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC.....'
};

await client.api('/informationProtection/threatAssessmentRequests')
    .version('beta')
    .post(threatAssessmentRequest);

```