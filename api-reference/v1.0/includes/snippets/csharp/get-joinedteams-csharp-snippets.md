---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fa6ace24c4504393915499730b35f04037500ee3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35473271"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var joinedTeams = await graphClient.Me.JoinedTeams
    .Request()
    .GetAsync();

```