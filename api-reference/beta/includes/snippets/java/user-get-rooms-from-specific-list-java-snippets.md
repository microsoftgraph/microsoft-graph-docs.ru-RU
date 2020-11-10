---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c44638a4fe745de1d579b2f1ca3afe61e3568dbf
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970131"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserFindRoomsCollectionPage findRooms = graphClient.me()
    .findRooms("Building2Rooms@contoso.onmicrosoft.com")
    .buildRequest()
    .get();

```