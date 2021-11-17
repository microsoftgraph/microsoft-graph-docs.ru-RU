---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 12feba81d01184b4f1e088387abdbacb018ea708246b140c2d4653510666b28c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57249659"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewSets = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].ReviewSets
    .Request()
    .GetAsync();

```