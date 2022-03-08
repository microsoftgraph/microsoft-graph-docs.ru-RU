---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: afa559a22610fca3f4671a12775be9a46b10fe3d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351741"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnPremisesAgentGroupCollectionPage agentGroups = graphClient.onPremisesPublishingProfiles("provisioning").agentGroups()
    .buildRequest()
    .expand("agents,publishedResources")
    .get();

```