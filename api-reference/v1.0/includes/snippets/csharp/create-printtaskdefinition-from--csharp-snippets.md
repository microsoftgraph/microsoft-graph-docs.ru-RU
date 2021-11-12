---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7d44c5d9219833af19b82201db85c280e8aadbd0c961d52a911ce69e12e191b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140300"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTaskDefinition = new PrintTaskDefinition
{
    DisplayName = "Test TaskDefinitionName",
    CreatedBy = new AppIdentity
    {
        DisplayName = "Requesting App Display Name"
    }
};

await graphClient.Print.TaskDefinitions
    .Request()
    .AddAsync(printTaskDefinition);

```