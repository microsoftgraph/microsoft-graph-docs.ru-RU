---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8a795fa85af86de39324ab6f726468ac13496861
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302640"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participants = new List<String>()
{
    ""
};

var clientContext = "clientContext-value";

await graphClient.Communications.Calls["{id}"].Participants
    .MuteAll(participants,clientContext)
    .Request()
    .PostAsync();

```