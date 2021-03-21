---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bcb929c6175df4a9a555a2903530c38409402988
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981473"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TemporaryAccessPassAuthenticationMethod temporaryAccessPassAuthenticationMethod = graphClient.users("kim@contoso.com").authentication().temporaryAccessPassMethods("30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30")
    .buildRequest()
    .get();

```