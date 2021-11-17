---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0d7ab1ac77c6aab94a52f36a95e72e5226e98f5de4c67b3382bc4b59022c529c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141778"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerRosterMember = await graphClient.Planner.Rosters["{plannerRoster-id}"].Members["{plannerRosterMember-id}"]
    .Request()
    .GetAsync();

```