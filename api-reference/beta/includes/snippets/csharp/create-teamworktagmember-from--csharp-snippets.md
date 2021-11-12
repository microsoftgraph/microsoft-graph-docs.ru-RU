---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 12afb7fd27828389b4098bd6313a988345ddde9c85fff691a3960c0ec7496070
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57262503"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamworkTagMember = new TeamworkTagMember
{
    UserId = "97f62344-57dc-409c-88ad-c4af14158ff5"
};

await graphClient.Teams["{team-id}"].Tags["{teamworkTag-id}"].Members
    .Request()
    .AddAsync(teamworkTagMember);

```