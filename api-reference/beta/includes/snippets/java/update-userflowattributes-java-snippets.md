---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ae8613eaf47ffed15e0c2025aaeb9fd6a4f69c35
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977088"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttribute identityUserFlowAttribute = new IdentityUserFlowAttribute();
identityUserFlowAttribute.description = "Your new hobby";

graphClient.identity().userFlowAttributes("extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby")
    .buildRequest()
    .patch(identityUserFlowAttribute);

```