---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d7ba1cc612fa1c0ab46f2e775168271a8b9aa48a
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66099552"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TemporaryAccessPassAuthenticationMethodCollectionPage temporaryAccessPassMethods = graphClient.users("071cc716-8147-4397-a5ba-b2105951cc0b").authentication().temporaryAccessPassMethods()
    .buildRequest()
    .get();

```