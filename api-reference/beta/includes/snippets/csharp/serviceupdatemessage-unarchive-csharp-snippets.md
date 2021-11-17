---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5ad67b03390b039a2403fa3cd2dbe54d79b2ec517907f1f8ce30a1393328a65c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57322422"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageIds = new List<String>()
{
    "MC172851",
    "MC167983"
};

await graphClient.Admin.ServiceAnnouncement.Messages
    .Unarchive(messageIds)
    .Request()
    .PostAsync();

```