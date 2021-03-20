---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6d26f4aefa27fbdfaf8d9ad59018dd01ec274052
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967663"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApplicationCollectionWithReferencesPage applications = graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups("{id}").applications()
    .buildRequest()
    .get();

```