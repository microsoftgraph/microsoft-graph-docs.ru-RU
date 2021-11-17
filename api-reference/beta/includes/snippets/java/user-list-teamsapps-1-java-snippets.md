---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 87f46301d3ad1ede09a209e624a79364e6757970fea8009b70ceae3257d700c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57264750"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserScopeTeamsAppInstallation userScopeTeamsAppInstallation = graphClient.users("{id}").teamwork().installedApps("{id}")
    .buildRequest()
    .get();

```