---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8ebc9394a197ce4cc6b75acaaf65d38405dbc996
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871336"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taughtClasses = await graphClient.Education.Users["{educationUser-id}"].TaughtClasses
    .Request()
    .GetAsync();

```