---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c5dd5288718d8643c63ddc05c3eb4743c80c180b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966775"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2cIdentityUserFlow b2cIdentityUserFlow = new B2cIdentityUserFlow();
b2cIdentityUserFlow.isLanguageCustomizationEnabled = true;
b2cIdentityUserFlow.defaultLanguageTag = "en";

graphClient.identity().b2cUserFlows("B2C_1_CustomerSignUp")
    .buildRequest()
    .patch(b2cIdentityUserFlow);

```