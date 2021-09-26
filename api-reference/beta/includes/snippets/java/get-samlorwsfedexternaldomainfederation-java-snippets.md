---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9802e209083ced5294c60e2992b864938bb328ed
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766580"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SamlOrWsFedExternalDomainFederationCollectionPage samlOrWsFedExternalDomainFederation = graphClient.directory().federationConfigurations().graph.samlOrWsFedExternalDomainFederation()
    .buildRequest()
    .filter("domains/any(x: x/id eq 'contoso.com')")
    .get();

```