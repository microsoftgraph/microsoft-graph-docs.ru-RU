---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c32508b762ccd537265692e88a5b2f07e912461d669c234f031fae5fdd2dfedf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57325273"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

var prompts = new List<Prompt>()
{
    new MediaPrompt
    {
        MediaInfo = new MediaInfo
        {
            Uri = "https://cdn.contoso.com/beep.wav",
            ResourceId = "1D6DE2D4-CD51-4309-8DAA-70768651088E"
        }
    }
};

await graphClient.Communications.Calls["{call-id}"]
    .PlayPrompt(prompts,clientContext)
    .Request()
    .PostAsync();

```