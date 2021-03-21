---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d3818ca15a7b9b029579708305a9718ab4326033
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972787"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WebAccount webAccount = new WebAccount();
webAccount.description = "My Github contributions!";
webAccount.userId = "innocenty.popov";
ServiceInformation service = new ServiceInformation();
service.name = "GitHub";
service.webUrl = "https://github.com";
webAccount.service = service;

graphClient.me().profile().webAccounts()
    .buildRequest()
    .post(webAccount);

```