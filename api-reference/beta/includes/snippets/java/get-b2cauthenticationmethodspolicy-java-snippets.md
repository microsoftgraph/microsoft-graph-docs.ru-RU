---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f21513e250b781976a0fe287f60cb5563ca8e73d2d89306332cc541c85525ebc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57195674"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2cAuthenticationMethodsPolicy b2cAuthenticationMethodsPolicy = graphClient.policies().b2cAuthenticationMethodsPolicy()
    .buildRequest()
    .get();

```