---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9e2f5bfbdde645a3dea45fcb7199216145490234
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763907"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalDomainName externalDomainName = new ExternalDomainName();
externalDomainName.id = "contososuites.com";

graphClient.directory().federationConfigurations("d5a56845-6845-d5a5-4568-a5d54568a5d5").microsoft.graph.samlOrWsFedExternalDomainFederation().domains()
    .buildRequest()
    .post(externalDomainName);

```