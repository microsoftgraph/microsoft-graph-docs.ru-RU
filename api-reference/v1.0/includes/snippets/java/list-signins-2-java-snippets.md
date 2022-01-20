---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d831da5fc1e0f3f92af56bcdf20d6aac1252e22b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128501"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("top", "10"));

SignInCollectionPage signIns = graphClient.auditLogs().signIns()
    .buildRequest( requestOptions )
    .filter("startsWith(appDisplayName,'Graph')")
    .get();

```