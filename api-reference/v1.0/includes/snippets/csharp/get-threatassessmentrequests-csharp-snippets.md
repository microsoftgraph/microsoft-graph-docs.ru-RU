---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 41cc85b945e59aadc2534fdbd37c82561f4c9b4b808c995b2a432dcf520be246
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140364"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequests = await graphClient.InformationProtection.ThreatAssessmentRequests
    .Request()
    .GetAsync();

```