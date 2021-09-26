---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 792ec7ef56da4a5bc6702ab80ec8e7b26e4390d7
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763759"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

ApplicationCollectionPage applications = graphClient.applications()
    .buildRequest( requestOptions )
    .filter("startswith(displayName, 'a')")
    .orderBy("displayName")
    .top(1)
    .get();

```