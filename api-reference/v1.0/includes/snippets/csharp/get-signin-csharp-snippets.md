---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 49fc36562ed06245a7a9f059c2f1808ad68f070b69d82669eba21432e75d9bc5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57198287"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var signIn = await graphClient.AuditLogs.SignIns["{signIn-id}"]
    .Request()
    .GetAsync();

```