---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 83bbc31e106f9558c3f54e8f3cc288e2b6da20d1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961821"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApplicationSignInDetailedSummary applicationSignInDetailedSummary = graphClient.reports().applicationSignInDetailedSummary("{id}")
    .buildRequest()
    .get();

```