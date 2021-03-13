---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dc9b9c83d8765723c32d89ca9aa5163b3fdb33be
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787539"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var orgContact = new OrgContact
{
    CompanyName = "companyName-value",
    Department = "department-value",
    DisplayName = "displayName-value",
    AdditionalData = new Dictionary<string, object>()
    {
        {"businessPhones", "[\"businessPhones-value\"]"},
        {"city", "city-value"},
        {"country", "country-value"}
    }
};

await graphClient.Contacts["{orgContact-id}"]
    .Request()
    .UpdateAsync(orgContact);

```