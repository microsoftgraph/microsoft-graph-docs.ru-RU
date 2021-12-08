---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 39662486de67172b9a39e55a0a4fad86ddcbe2b2
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346031"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InsightsSettings insightsSettings = graphClient.organization("{organizationId}").settings().peopleInsights()
    .buildRequest()
    .get();

```