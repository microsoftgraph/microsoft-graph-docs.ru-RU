---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: efdb47c7b165d5d3af61da2510856b4c4684692e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210345"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TenantRelationships.DelegatedAdminRelationships["{delegatedAdminRelationship-id}"].AccessAssignments["{delegatedAdminAccessAssignment-id}"]
    .Request()
    .Header("If-Match","W/\"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw==\"")
    .DeleteAsync();

```