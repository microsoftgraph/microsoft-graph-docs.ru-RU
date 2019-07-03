---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 589b3b16ea4adbb15d1dda5e354fdfdeff4ffdaa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35473502"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageRule = new MessageRule
{
    DisplayName = "Important from partner",
    Actions = new MessageRuleActions
    {
        MarkImportance = Importance.High
    }
};

await graphClient.Me.MailFolders["inbox"].MessageRules["AQAAAJ5dZqA="]
    .Request()
    .UpdateAsync(messageRule);

```