---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d087a16cc58f05d9abf6f99660252b3edcd49e6e7356d48b44e4b78751762450
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143023"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Admin.ServiceAnnouncement.Issues["{serviceHealthIssue-id}"]
    .IncidentReport()
    .Request()
    .GetAsync();

```