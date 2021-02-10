---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 03b8752fe801f9c1fc08c98e6de0fb43dd9e87fa
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179281"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Filter("endswith(mail,'a@contoso.com')")
    .OrderBy("userPrincipalName")
    .GetAsync();

```