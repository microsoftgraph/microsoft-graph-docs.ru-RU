---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 817af4dd53032b1c384ffe884c310b1ce1b779c7ff064c273672ced7eb28e198
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57309407"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printOperation = await graphClient.Print.Operations["{printOperation-id}"]
    .Request()
    .GetAsync();

```