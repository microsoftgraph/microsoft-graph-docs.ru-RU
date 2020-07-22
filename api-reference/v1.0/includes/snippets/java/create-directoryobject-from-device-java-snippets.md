---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 64cdf2923336fe3a6ea433670c6aef09c9e3face
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2020
ms.locfileid: "45224581"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.Id = "{id}";

graphClient.devices("{id}").registeredUsers().references()
    .buildRequest()
    .post(directoryObject);

```