---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9a28be6fdf4ea6dd0ca531d3a6d0dbadec76fde3
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692871"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserCollectionWithReferencesPage allowedUsers = graphClient.print().shares("{id}").allowedUsers()
    .buildRequest()
    .get();

```