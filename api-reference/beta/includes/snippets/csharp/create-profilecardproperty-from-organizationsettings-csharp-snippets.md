---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 81cad6401df12cc8dd8c454ece4015b3a6f6d1d538f3413ea637363baa584043
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57196242"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profileCardProperty = new ProfileCardProperty
{
    DirectoryPropertyName = "CustomAttribute1",
    Annotations = new List<ProfileCardAnnotation>()
    {
        new ProfileCardAnnotation
        {
            DisplayName = "Cost Center",
            Localizations = new List<DisplayNameLocalization>()
            {
                new DisplayNameLocalization
                {
                    LanguageTag = "ru-RU",
                    DisplayName = "центр затрат"
                }
            }
        }
    }
};

await graphClient.Organization["{organization-id}"].Settings.ProfileCardProperties
    .Request()
    .AddAsync(profileCardProperty);

```