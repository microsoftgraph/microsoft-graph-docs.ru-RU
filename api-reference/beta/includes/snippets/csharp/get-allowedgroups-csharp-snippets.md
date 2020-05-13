---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 14b9e9b7c7b22843e5ead0fcb9651bef62358dd7
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216863"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var allowedGroups = await graphClient.Print.Shares["{id}"].AllowedGroups
    .Request()
    .GetAsync();

```