---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1dee22f5c83ce4f6d69e3e6a3d592b3f6d0e0faeeb0d94019403c97bdc78ffca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57198836"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var fido2AuthenticationMethod = await graphClient.Me.Authentication.Fido2Methods["{fido2AuthenticationMethod-id}"]
    .Request()
    .GetAsync();

```