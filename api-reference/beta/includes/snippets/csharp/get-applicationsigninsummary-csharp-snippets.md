---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0e8b3c1bef2c97260b3f159a7afb349c59b51d24e700cb027f70642189c885db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57051627"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getAzureADApplicationSignInSummary = await graphClient.Reports
    .GetAzureADApplicationSignInSummary("D7")
    .Request()
    .GetAsync();

```