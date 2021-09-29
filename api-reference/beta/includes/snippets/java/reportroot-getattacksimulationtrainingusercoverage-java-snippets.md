---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 57a3024455605b42032299939c4cadcc3b7c0822
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/29/2021
ms.locfileid: "59997200"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRootGetAttackSimulationTrainingUserCoverageCollectionPage getAttackSimulationTrainingUserCoverage = graphClient.reports()
    .getAttackSimulationTrainingUserCoverage()
    .buildRequest()
    .get();

```