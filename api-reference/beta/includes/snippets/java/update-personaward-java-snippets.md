---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a28e07c8b4bbcee8ff50b849b96932c6c8c41fb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774112"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAward personAward = new PersonAward();
personAward.issuingAuthority = "International Association of Branding Management";
personAward.thumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg";

graphClient.users("{userId}").profile().awards("{personAwardId}")
    .buildRequest()
    .patch(personAward);

```