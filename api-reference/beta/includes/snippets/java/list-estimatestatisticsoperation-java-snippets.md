---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 637067dcefd48c5dd92db9f578b319015f6b4bb1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772606"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EstimateStatisticsOperation estimateStatisticsOperation = graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("95bdbf84f02f4bdaafbbb2fe945a4962").lastEstimateStatisticsOperation()
    .buildRequest()
    .get();

```