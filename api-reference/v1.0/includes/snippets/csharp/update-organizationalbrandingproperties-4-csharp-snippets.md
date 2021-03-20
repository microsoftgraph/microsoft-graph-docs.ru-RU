---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 244a12cae3af765a40b980acada5d3c9254442c0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949401"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBranding = new OrganizationalBranding
{
    BackgroundColor = "#FFFF33"
};

await graphClient.Organization["{organization-id}"].Branding
    .Request()
    .PutAsync(organizationalBranding);

```