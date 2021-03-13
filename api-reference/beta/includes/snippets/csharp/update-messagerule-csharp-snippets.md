---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cc63868fd3553b200013cce047ca410eb8df63bd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784305"
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

await graphClient.Me.MailFolders["{mailFolder-id}"].MessageRules["{messageRule-id}"]
    .Request()
    .UpdateAsync(messageRule);

```