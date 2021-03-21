---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 31fa80260aa03447bd483f8042e1be58af61d34f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979798"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRootGetCredentialUsageSummaryCollectionPage getCredentialUsageSummary = graphClient.reports()
    .getCredentialUsageSummary(ReportRootGetCredentialUsageSummaryParameterSet
        .newBuilder()
        .withPeriod("D30")
        .build())
    .buildRequest()
    .filter("feature eq 'registration'")
    .get();

```