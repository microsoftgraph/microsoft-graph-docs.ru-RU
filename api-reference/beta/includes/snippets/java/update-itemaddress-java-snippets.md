---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 87f58890a1dd384f6d292f3fe83a164193d3282a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774666"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemAddress itemAddress = new ItemAddress();
itemAddress.allowedAudiences = EnumSet.of(AllowedAudiences.ME);
itemAddress.displayName = "Secret Hideout";

graphClient.users("{userId}").profile().addresses("{id}")
    .buildRequest()
    .patch(itemAddress);

```