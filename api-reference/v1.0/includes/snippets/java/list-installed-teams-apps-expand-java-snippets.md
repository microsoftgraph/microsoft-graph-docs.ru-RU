---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a790b8bea8bda072d64c95e507a6a436ae886adc600de1dde114671f97ed3f76
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57396756"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallationCollectionPage installedApps = graphClient.teams("6903fa93-605b-43ef-920e-77c4729f8258").installedApps()
    .buildRequest()
    .expand("teamsAppDefinition")
    .get();

```