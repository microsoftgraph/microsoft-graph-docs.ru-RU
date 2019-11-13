---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f91c9f0f767ce046c433aaa2afd2d91930119635
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302381"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callbackUri = "callbackUri-value";

var mediaConfig = new AppHostedMediaConfig
{
    Blob = "<Media Session Configuration Blob>"
};

var acceptedModalities = new List<Modality>()
{
    Modality.Audio
};

await graphClient.Communications.Calls["{id}"]
    .Answer(callbackUri,mediaConfig,acceptedModalities)
    .Request()
    .PostAsync();

```