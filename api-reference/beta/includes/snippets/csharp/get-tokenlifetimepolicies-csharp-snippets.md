---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4cf2749aefc922f121ef9ca2c2aa3594a150c8b0208fcabe98d7d48f460013b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57364602"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicies = await graphClient.Policies.TokenLifetimePolicies
    .Request()
    .GetAsync();

```