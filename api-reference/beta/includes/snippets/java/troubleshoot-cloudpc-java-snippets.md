---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f3474285225b714ffb914e2bb5af46eb328a677c
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61523727"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.deviceManagement().virtualEndpoint().cloudPCs("ff4eb6ab-d56a-4edf-90c1-baaec8dd6032")
    .troubleshoot()
    .buildRequest()
    .post();

```