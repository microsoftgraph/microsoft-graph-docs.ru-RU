---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 877cd7607df104ff2e387ebc35b24ae8139547ce
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209036"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

GroupCollectionPage group = graphClient.groups("{id}").memberOf().microsoft.graph.group()
    .buildRequest( requestOptions )
    .filter("startswith(displayName, 'A')")
    .orderBy("displayName")
    .get();

```