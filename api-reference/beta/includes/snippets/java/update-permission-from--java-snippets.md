---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9a93d81237cbee426459a45fd7db26165a5b27d0
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177287"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Permission permission = new Permission();
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("read");
permission.roles = rolesList;

graphClient.sites("{sitesId}").permissions("{permissionId}")
    .buildRequest()
    .patch(permission);

```