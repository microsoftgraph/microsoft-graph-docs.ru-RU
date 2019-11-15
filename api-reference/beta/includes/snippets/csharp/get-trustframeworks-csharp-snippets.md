---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1d592a63a4876e6220ef8b514cb38874e230708a
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "35716761"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var policies = await graphClient.TrustFramework.Policies
    .Request()
    .GetAsync();

```