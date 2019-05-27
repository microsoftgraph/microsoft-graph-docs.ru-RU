---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eac21e21b84c269c7875d567c33362e2be77c26d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448015"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var overrides = await graphClient.Me.InferenceClassification.Overrides
    .Request()
    .GetAsync();

```