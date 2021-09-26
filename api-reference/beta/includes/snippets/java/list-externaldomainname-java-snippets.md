---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 75cedf7603d26f12ce25a2992f3f8bb7ef048fd2
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766538"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalDomainNameCollectionPage domains = graphClient.directory().federationConfigurations().microsoft.graph.samlOrWsFedExternalDomainFederation("f1e11a04-0244-4592-99df-b01cfaadce15").domains()
    .buildRequest()
    .get();

```