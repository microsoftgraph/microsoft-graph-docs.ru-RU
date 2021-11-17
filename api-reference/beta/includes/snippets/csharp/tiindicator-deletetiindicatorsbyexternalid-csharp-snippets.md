---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7fca1516086bbc485c37bd72a8483416267228f6b0b4e4e73b68b5d6002fdebb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143304"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<String>()
{
    "externalId-value1",
    "externalId-value2"
};

await graphClient.Security.TiIndicators
    .DeleteTiIndicatorsByExternalId(value)
    .Request()
    .PostAsync();

```