---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5d777de71d106f87b5c57fe42fcce8bb23f3d149
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821259"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationalActivity = new EducationalActivity
{
    Institution = new InstitutionData
    {
        Location = new PhysicalAddress
        {
            Type = PhysicalAddressType.Business,
            PostOfficeBox = null,
            Street = "12000 E Prospect Rd",
            City = "Fort Collins",
            State = "Colorado",
            CountryOrRegion = "USA",
            PostalCode = "80525"
        }
    }
};

await graphClient.Me.Profile.EducationalActivities["{id}"]
    .Request()
    .UpdateAsync(educationalActivity);

```