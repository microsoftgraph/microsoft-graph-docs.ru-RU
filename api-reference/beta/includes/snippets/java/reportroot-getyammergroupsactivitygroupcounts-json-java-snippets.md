---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 129207cb3e3b527672d21f49a32aa0e8c98dbbce
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358403"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerGroupsActivityGroupCountsCollectionPage getYammerGroupsActivityGroupCounts = graphClient.reports()
    .getYammerGroupsActivityGroupCounts("D7")
    .buildRequest()
    .get();

```