---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3583bac0a86ff748a4058c503f44cc331b322f76fd866950ea1340e934ba6229
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050635"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var certificateBasedAuthConfiguration = await graphClient.Organization["{organization-id}"].CertificateBasedAuthConfiguration["{certificateBasedAuthConfiguration-id}"]
    .Request()
    .GetAsync();

```