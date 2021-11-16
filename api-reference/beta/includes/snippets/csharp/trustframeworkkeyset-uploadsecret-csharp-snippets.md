---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 79e22167726fa0011396e6966850fa06eee13b54435818510bbedd0a7576b9a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57255902"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var use = "use-value";

var k = "application-secret-to-be-uploaded";

var nbf = 1508969811;

var exp = 1508973711;

await graphClient.TrustFramework.KeySets["{trustFrameworkKeySet-id}"]
    .UploadSecret(use,k,nbf,exp)
    .Request()
    .PostAsync();

```