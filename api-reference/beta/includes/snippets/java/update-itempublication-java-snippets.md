---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f53332254d79aeb2609d5a3cde20e1482d4c5a72
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770376"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPublication itemPublication = new ItemPublication();
itemPublication.publisher = "International Association of Branding Management Publishing";
itemPublication.thumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg";

graphClient.users("{userId}").profile().publications("{id}")
    .buildRequest()
    .patch(itemPublication);

```