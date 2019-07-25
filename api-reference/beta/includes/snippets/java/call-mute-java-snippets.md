---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 62d293909bbdcfb8f55975ea755b6963d7eb5eaf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864737"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "clientContext-value";

graphClient.app().calls("{id}")
    .mute(clientContext)
    .buildRequest()
    .post();

```