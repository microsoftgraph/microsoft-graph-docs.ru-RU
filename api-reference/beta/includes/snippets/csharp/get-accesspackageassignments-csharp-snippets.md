---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9a78b4ba25b6ecf949652da74b2e7a14785ee33b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "37993038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignments = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignments
    .Request()
    .GetAsync();

```