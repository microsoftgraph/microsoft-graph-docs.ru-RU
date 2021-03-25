---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bb578cec4c4cf42f92272489fc6b04573211806c
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210885"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordlessMicrosoftAuthenticatorAuthenticationMethodCollectionPage passwordlessMicrosoftAuthenticatorMethods = graphClient.me().authentication().passwordlessMicrosoftAuthenticatorMethods()
    .buildRequest()
    .get();

```