---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 44a76ce9fc39d542eb82968db3deff870f533294
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975221"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.displayName = "Rogelio Cazares";
educationUser.givenName = "Rogelio";
educationUser.middleName = "Fernando";
educationUser.surname = "Cazares";

graphClient.education().users("13020")
    .buildRequest()
    .patch(educationUser);

```