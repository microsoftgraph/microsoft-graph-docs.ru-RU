---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 553a6957e93222a41b461648684859eebd860fa1
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "47413367"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"members@odata.bind", "[\"https://graph.microsoft.com/v1.0/directoryObjects/{id}\",\"https://graph.microsoft.com/v1.0/directoryObjects/{id}\",\"https://graph.microsoft.com/v1.0/directoryObjects/{id}\"]"}
    }
};

await graphClient.Groups["{group-id}"]
    .Request()
    .UpdateAsync(group);

```