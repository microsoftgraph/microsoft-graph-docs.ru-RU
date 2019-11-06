---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4c689230cd9d228e9071e09f8a329ef6f4d003a6
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997979"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var interests = await graphClient.Me.Profile.Interests
    .Request()
    .GetAsync();

```