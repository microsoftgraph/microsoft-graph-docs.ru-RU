---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 64215f446ab412daf4ba233663f681d5f39f763c
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905273"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var devices = await graphClient.Devices
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:Android")
    .GetAsync();

```