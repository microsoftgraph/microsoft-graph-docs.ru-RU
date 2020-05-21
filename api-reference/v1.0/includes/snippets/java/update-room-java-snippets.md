---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f0b9e592a149737696c96c9902353709e963c3e2
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336399"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Room place = new Room();
place.nickname = "Conf Room";
place.building = "1";
place.label = "100";
place.capacity = "50";
place.isWheelchairAccessible = false;

graphClient.places("cf100@contoso.com")
    .buildRequest()
    .patch(place);

```