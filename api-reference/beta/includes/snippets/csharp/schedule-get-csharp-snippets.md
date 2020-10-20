---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 668dd8b1a440b3a2d9e59df6fc41ac0b85ff80ae
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611039"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schedule = await graphClient.Teams["{teamId}"].Schedule
    .Request()
    .GetAsync();

```