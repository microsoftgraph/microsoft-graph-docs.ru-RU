---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f5e0bcb10245e3fc439abf6f1634473e25fcedc1cb9ddc37229eef26d4734934
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57430891"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBase identityProviderBase = graphClient.identity().identityProviders("MSASignup-OAUTH")
    .buildRequest()
    .get();

```