---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8af666292e54e34b9997dcccf121345ba032e21a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220699"
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

var callOptions = new IncomingCallOptions
{
    IsContentSharingNotificationEnabled = true
};

var participantCapacity = 200;

await graphClient.Communications.Calls["{call-id}"]
    .Answer(callbackUri,mediaConfig,acceptedModalities,participantCapacity,callOptions)
    .Request()
    .PostAsync();

```