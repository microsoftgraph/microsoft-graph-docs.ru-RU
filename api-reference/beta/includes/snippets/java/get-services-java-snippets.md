---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: be89f9351dc996b01b6b64f05002de8a46cbe33f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789451"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IBookingServiceCollectionPage services = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").services()
    .buildRequest()
    .get();

```