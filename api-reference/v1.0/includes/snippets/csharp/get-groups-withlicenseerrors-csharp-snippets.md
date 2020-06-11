---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d6f8ed14ecc521b60bc6a3ff2ad620e2fe43f8b5
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683670"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
    .Request()
    .Filter("hasMembersWithLicenseErrors+eq+true,")
    .Select("id,displayName")
    .GetAsync();

```