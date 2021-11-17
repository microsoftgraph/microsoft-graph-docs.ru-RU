---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ba7e8a845685880b369b6defdd4f83cc59e492672a0fb6d474722baa57cd3078
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57365499"
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

await graphClient.Me.Profile.EducationalActivities["{educationalActivity-id}"]
    .Request()
    .UpdateAsync(educationalActivity);

```