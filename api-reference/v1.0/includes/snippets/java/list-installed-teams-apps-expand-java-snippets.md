---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 502077b066a152e71cbba986d337341b0a68b8fc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963656"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallationCollectionPage installedApps = graphClient.teams("6903fa93-605b-43ef-920e-77c4729f8258").installedApps()
    .buildRequest()
    .expand("teamsAppDefinition")
    .get();

```