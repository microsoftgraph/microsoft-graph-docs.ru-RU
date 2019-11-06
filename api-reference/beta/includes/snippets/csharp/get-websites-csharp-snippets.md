---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: db315679cbafe4cf482b2684c5a40dcaacac14ea
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997886"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var websites = await graphClient.Me.Profile.Websites
    .Request()
    .GetAsync();

```