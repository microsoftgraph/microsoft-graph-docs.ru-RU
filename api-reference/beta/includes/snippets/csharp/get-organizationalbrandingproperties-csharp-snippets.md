---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: af322bca1c0486b0f9fbcfdbec1251427ade10dc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785897"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBrandingLocalization = new OrganizationalBrandingLocalization
{
    BackgroundColor = "#00000F",
    Id = "fr"
};

await graphClient.Organization["{organization-id}"].Branding.Localizations
    .Request()
    .AddAsync(organizationalBrandingLocalization);

```