---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1c2f1d5cffffda621358bb34bc5e63cecbea4100
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956543"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UrlAssessmentRequest threatAssessmentRequest = new UrlAssessmentRequest();
threatAssessmentRequest.url = "http://test.com";
threatAssessmentRequest.expectedAssessment = ThreatExpectedAssessment.BLOCK;
threatAssessmentRequest.category = ThreatCategory.PHISHING;

graphClient.informationProtection().threatAssessmentRequests()
    .buildRequest()
    .post(threatAssessmentRequest);

```