---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7f0cdc214595b2eaad2293349fb3319dfb28e964
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201738"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppConsentRequest appConsentRequest = graphClient.identityGovernance().appConsent().appConsentRequests("af330b30-dd59-4482-a848-0fd81b0438ed")
    .buildRequest()
    .get();

```