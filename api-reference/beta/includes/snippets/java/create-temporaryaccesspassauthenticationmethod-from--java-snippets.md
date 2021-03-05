---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 90a65b15bdced879fe453eb7b126e363ef4d3da9
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475121"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TemporaryAccessPassAuthenticationMethod temporaryAccessPassAuthenticationMethod = new TemporaryAccessPassAuthenticationMethod();
temporaryAccessPassAuthenticationMethod.startDateTime = CalendarSerializer.deserialize("2021-01-26T00:00:00Z");
temporaryAccessPassAuthenticationMethod.lifetimeInMinutes = 60;
temporaryAccessPassAuthenticationMethod.isUsableOnce = false;

graphClient.users("kim@contoso.com").authentication().temporaryAccessPassMethods()
    .buildRequest()
    .post(temporaryAccessPassAuthenticationMethod);

```