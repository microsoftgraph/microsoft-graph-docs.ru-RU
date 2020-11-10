---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c8db06b901d7d2cc5c690bdd4c2b9f035598e2eb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973394"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPublishedResourceCollectionPage publishedResources = graphClient.onPremisesPublishingProfiles("{publishingType}").publishedResources()
    .buildRequest()
    .expand("agentGroups")
    .get();

```