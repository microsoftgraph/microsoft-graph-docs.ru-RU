---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bfbf663d1bad845676754df9d25b6d6a4f87c017
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967948"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.onPremisesPublishingProfiles("provisioning").agents("1234b780-965f-4149-85c5-a8c73e58b67d").agentGroups("8832388F-3814-4952-B288-FFB62081FE25").reference()
    .buildRequest()
    .delete();

```