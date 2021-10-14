---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9d367fa3c724159508d57f7690d35f803799464d3dd7beac5da1b6248004746c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57053215"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallation teamsAppInstallation = graphClient.teams("{id}").installedApps("{id}")
    .buildRequest()
    .expand("teamsAppDefinition")
    .get();

```