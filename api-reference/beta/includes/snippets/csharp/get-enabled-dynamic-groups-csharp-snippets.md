---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 27e38522c9036ebd5636a354e5edf79099e72d2c
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528814"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var groups = await graphClient.Groups
    .Request( queryOptions )
    .Filter("mailEnabled eq false and securityEnabled eq true and NOT(groupTypes/any(s:s eq 'Unified')) and membershipRuleProcessingState eq 'On'")
    .Select("id,membershipRule,membershipRuleProcessingState")
    .GetAsync();

```