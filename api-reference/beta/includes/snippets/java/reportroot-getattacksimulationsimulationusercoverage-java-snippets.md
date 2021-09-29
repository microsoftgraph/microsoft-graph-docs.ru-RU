---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e0500a4fb7fbeb7b48377a74b886c6489abc37b3
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996403"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRootGetAttackSimulationSimulationUserCoverageCollectionPage getAttackSimulationSimulationUserCoverage = graphClient.reports()
    .getAttackSimulationSimulationUserCoverage()
    .buildRequest()
    .get();

```