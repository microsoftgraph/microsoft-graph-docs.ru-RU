---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ce54b3e2928d8417c095f3e23b7544a88e01800d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982695"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PublishedResourceCollectionPage publishedResources = graphClient.onPremisesPublishingProfiles("{publishingType}").publishedResources()
    .buildRequest()
    .expand("agentGroups")
    .get();

```