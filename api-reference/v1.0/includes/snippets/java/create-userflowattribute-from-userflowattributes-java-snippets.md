---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2e33cf448360b5f3597cae99daa30587c8205f75a99f5a7738c99fe2ff58c4c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57205273"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttribute identityUserFlowAttribute = new IdentityUserFlowAttribute();
identityUserFlowAttribute.displayName = "Hobby";
identityUserFlowAttribute.description = "Your hobby";
identityUserFlowAttribute.dataType = IdentityUserFlowAttributeDataType.STRING;

graphClient.identity().userFlowAttributes()
    .buildRequest()
    .post(identityUserFlowAttribute);

```