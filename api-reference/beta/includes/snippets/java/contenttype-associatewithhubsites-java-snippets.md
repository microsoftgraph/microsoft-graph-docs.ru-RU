---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9a1b310caf93981c7d8541a640253c03c1eadb4f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771143"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> hubSiteUrlsList = new LinkedList<String>();
hubSiteUrlsList.add("https://graph.microsoft.com/beta/sites/id");

Boolean propagateToExistingLists = false;

graphClient.sites("id").contentTypes("id")
    .associateWithHubSites(hubSiteUrlsList,propagateToExistingLists)
    .buildRequest()
    .post();

```