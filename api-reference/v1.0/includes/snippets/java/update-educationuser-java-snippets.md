---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8f2a3a412a64b1ead425980eb8509c8b3a89049629314f7d137ed736323d62db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141866"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.displayName = "Rogelio Cazares";
educationUser.givenName = "Rogelio";
educationUser.middleName = "Fernando";
educationUser.surname = "Cazares";

graphClient.education().users("{user-id}")
    .buildRequest()
    .patch(educationUser);

```