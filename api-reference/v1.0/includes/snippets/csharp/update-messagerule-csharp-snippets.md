---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f06b4f7dde2019df4c87edab96631e0a235f203c76672d98d08a9cb7e420ea4f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57251233"
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