---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 139fa80f71538c1c3bce37102beba299e7e06a2d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604063"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkAGE1M2_bs88AACHsLqWAAA="]
    .Request()
    .Filter("id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color')")
    .Expand("singleValueExtendedProperties($filter=id%20eq%20'String%20%7B66f5a359-4659-4830-9070-00047ec6ac6e%7D%20Name%20Color')")
    .GetAsync();

```