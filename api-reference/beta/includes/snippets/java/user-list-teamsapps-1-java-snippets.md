---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 80750f25a502310e9a17d20e9bf881491a667262
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955099"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserScopeTeamsAppInstallation userScopeTeamsAppInstallation = graphClient.users("{id}").teamwork().installedApps("{id}")
    .buildRequest()
    .get();

```