---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b286e8671dcb7f9fd254ae25841aceac93278e9dcc8034ad94f28eabdccfb716
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57202184"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personCertification = new PersonCertification
{
    IssuingAuthority = "International Academy of Marketing Excellence",
    IssuingCompany = "International Academy of Marketing Excellence"
};

await graphClient.Users["{user-id}"].Profile.Certifications["{personCertification-id}"]
    .Request()
    .UpdateAsync(personCertification);

```