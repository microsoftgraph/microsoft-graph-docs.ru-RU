---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bc7b418a888f3ca737c90cee60f10cf3c0a4fbef
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359529"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessDeviceUsageDistributionUserCountsCollectionPage getSkypeForBusinessDeviceUsageDistributionUserCounts = graphClient.reports()
    .getSkypeForBusinessDeviceUsageDistributionUserCounts("D7")
    .buildRequest()
    .get();

```