---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ebfd9bcac4f8f88c33ee9c24fe1c5c8081cde83c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955306"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var analytics = await graphClient.Me.Analytics
    .Request()
    .Select("Settings")
    .GetAsync();

var settings = analytics.Settings;

```