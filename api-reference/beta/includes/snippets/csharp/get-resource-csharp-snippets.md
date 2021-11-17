---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6d68cc982e472900c4384e1fe497e0ed5fcbbdcb7dd49bbab6ce60c3d63601f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57051927"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Me.Onenote.Resources["{onenoteResource-id}"].Content
    .Request()
    .GetAsync();

```