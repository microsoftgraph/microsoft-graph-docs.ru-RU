---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1eb5b9f04f0c49e28bd8f81c138a7cbdf4d9b059
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943837"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

using var stream = new System.IO.MemoryStream(Encoding.UTF8.GetBytes(@"<Image>"));

await graphClient.Organization["{organization-id}"].Branding.Localizations["{organizationalBrandingLocalization-id}"].BannerLogo
    .Request()
    .PutAsync<OrganizationalBrandingLocalization>(stream);

```