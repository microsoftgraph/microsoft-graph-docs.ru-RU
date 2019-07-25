---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2c37f0283ded5d22785ca2b92108bdba45faad1f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871283"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerGroupsActivityGroupCountsCollectionPage getYammerGroupsActivityGroupCounts = graphClient.reports()
    .getYammerGroupsActivityGroupCounts('D7')
    .buildRequest()
    .get();

```