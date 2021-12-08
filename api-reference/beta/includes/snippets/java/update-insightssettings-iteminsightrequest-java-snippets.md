---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1edf8517e6a7838c079b821edd09b2e2d681d472
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61339551"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InsightsSettings insightsSettings = new InsightsSettings();
insightsSettings.disabledForGroup = "edbfe4fb-ec70-4300-928f-dbb2ae86c981";

graphClient.organization("{organizationId}").settings().itemInsights()
    .buildRequest()
    .patch(insightsSettings);

```