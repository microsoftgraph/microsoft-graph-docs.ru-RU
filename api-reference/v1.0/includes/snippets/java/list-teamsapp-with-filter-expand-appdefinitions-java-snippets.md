---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2dab47d9a0b03b7528cf1daeca73a35d990b839dc4a001876adee27d37e0b639
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57255309"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest()
    .filter("id eq '876df28f-2e78-423b-94a5-44181bd0e225'")
    .expand("appDefinitions")
    .get();

```