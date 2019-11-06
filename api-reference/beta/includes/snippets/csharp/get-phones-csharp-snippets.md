---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5489bb36330b53d55e505764c7f967bc6c50a6eb
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996911"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var phones = await graphClient.Me.Profile.Phones
    .Request()
    .GetAsync();

```