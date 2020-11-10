---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1b6b84552d6322a00b76ba32b2bf7d4d38b7020a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976911"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnPremisesPublishingProfile onPremisesPublishingProfile = graphClient.onPremisesPublishingProfiles("provisioning")
    .buildRequest()
    .expand("agentGroups")
    .get();

```