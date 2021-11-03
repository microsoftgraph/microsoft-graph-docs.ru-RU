---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d0fa1ca71d6625157e75a8f514e06b90f7e367ee
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730335"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recoveryKeys = await graphClient.InformationProtection.Bitlocker.RecoveryKeys
    .Request()
    .Header("ocp-client-name","\"My Friendly Client\"")
    .Header("ocp-client-version","\"1.2\"")
    .GetAsync();

```