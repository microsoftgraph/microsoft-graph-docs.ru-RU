---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f3908636f9b7a9c500017def6fab8f09775b75f1
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442772"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TemporaryAccessPassAuthenticationMethodConfiguration authenticationMethodConfiguration = new TemporaryAccessPassAuthenticationMethodConfiguration();
authenticationMethodConfiguration.isUsableOnce = true;

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("temporaryAccessPass")
    .buildRequest()
    .patch(authenticationMethodConfiguration);

```