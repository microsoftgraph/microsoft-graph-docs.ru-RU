---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff76b0bc66cb5b590b373a92180c8bbd73ccf6f2f65dbc050a87a5e8aa700ab4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57372089"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].InstalledApps["{teamsAppInstallation-id}"]
    .Upgrade()
    .Request()
    .PostAsync();

```