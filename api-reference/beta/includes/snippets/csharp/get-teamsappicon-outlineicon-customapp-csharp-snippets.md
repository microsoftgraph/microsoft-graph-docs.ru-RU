---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dd238464cbea2ae0bf6f2405a5469b2ade173289aab793b6c71f3fb0cc167e0f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57207491"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppIcon = await graphClient.AppCatalogs.TeamsApps["{teamsApp-id}"].AppDefinitions["{teamsAppDefinition-id}"].OutlineIcon
    .Request()
    .GetAsync();

```