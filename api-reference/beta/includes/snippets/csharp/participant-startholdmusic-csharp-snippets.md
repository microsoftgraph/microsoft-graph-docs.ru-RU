---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 80ccccab3c9e384af20c6219e8be1772084ee75d
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507315"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customPrompt = new MediaPrompt
{
    MediaInfo = new MediaInfo
    {
        Uri = "https://bot.contoso.com/onHold.wav"
    }
};

var clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

await graphClient.Communications.Calls["{call-id}"].Participants["{participant-id}"]
    .StartHoldMusic(customPrompt,clientContext)
    .Request()
    .PostAsync();

```