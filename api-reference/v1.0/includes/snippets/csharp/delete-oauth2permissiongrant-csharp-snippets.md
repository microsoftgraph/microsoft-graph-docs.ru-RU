---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d560de9e95612e2195314451939e9425cf2e74a2a825ba4b54d5382e3ac80598
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57310887"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Oauth2PermissionGrants["{oAuth2PermissionGrant-id}"]
    .Request()
    .DeleteAsync();

```