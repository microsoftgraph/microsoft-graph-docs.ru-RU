---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 627bb69f7588333341e1a57f3dccdf5ce470df27
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978906"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EstimateStatisticsOperation estimateStatisticsOperation = graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("95bdbf84f02f4bdaafbbb2fe945a4962").lastEstimateStatisticsOperation()
    .buildRequest()
    .get();

```