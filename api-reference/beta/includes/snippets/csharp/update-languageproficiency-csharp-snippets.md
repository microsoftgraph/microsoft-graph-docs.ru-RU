---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a2f180d3c647d437c2ad838cfb9ab84a22f876ad
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782181"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languageProficiency = new LanguageProficiency
{
    AllowedAudiences = AllowedAudiences.Organization
};

await graphClient.Me.Profile.Languages["{languageProficiency-id}"]
    .Request()
    .UpdateAsync(languageProficiency);

```