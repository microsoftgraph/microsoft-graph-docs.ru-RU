---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9a7e7c5db7d81a958c3435fe90abafb4d4064fbd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871499"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerDeviceUsageDistributionUserCountsCollectionPage getYammerDeviceUsageDistributionUserCounts = graphClient.reports()
    .getYammerDeviceUsageDistributionUserCounts('D7')
    .buildRequest()
    .get();

```