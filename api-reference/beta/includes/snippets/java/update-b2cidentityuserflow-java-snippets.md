---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b827259622a50b3af0671ed25ad34b89eadb61d3
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843662"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2cIdentityUserFlow b2cIdentityUserFlow = new B2cIdentityUserFlow();
b2cIdentityUserFlow.isLanguageCustomizationEnabled = true;
b2cIdentityUserFlow.defaultLanguageTag = "en";

graphClient.identity().b2cUserFlows("B2C_1_CustomerSignUp")
    .buildRequest()
    .patch(b2cIdentityUserFlow);

```