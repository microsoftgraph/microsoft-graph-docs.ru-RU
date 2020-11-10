---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0bf95d7cce61e2e7174a84f6f29360e05c451c1f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976968"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnPremisesAgentGroup onPremisesAgentGroup = graphClient.onPremisesPublishingProfiles("provisioning").agentGroups("2d55ed41-1619-4848-92bb-0576d3038682")
    .buildRequest()
    .expand("agents")
    .get();

```