---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0a65078cd38656fee3d2f83c241029441bd07b0d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976798"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFindRoomsCollectionPage findRooms = graphClient.me()
    .findRooms(UserFindRoomsParameterSet
        .newBuilder()
        .withRoomList("Building2Rooms@contoso.onmicrosoft.com")
        .build())
    .buildRequest()
    .get();

```