---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7acab4e1ff487d5d8f43304e5edaf796eb3e028363b36d8509f3c97f02082c1e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57207895"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=minimal"));

GroupDeltaCollectionPage delta = graphClient.groups()
    .delta()
    .buildRequest( requestOptions )
    .select("displayName,description,mailNickname")
    .get();

```