---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: de272c13eb9ab987afedea43aee0ff7deec394532205c859b89f677f069e3edd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57055254"
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