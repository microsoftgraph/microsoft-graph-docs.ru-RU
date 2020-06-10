---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ebfd9bcac4f8f88c33ee9c24fe1c5c8081cde83c
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684746"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var analytics = await graphClient.Me.Analytics
    .Request()
    .Select("Settings")
    .GetAsync();

var settings = analytics.Settings;

```