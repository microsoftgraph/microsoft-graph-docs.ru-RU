---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 32bbfd0ff866caab644af9e0f571d3378251de14
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205124"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleRequest unifiedRoleAssignmentScheduleRequest = graphClient.roleManagement().directory().roleAssignmentScheduleRequests("95c690fb-3eb3-4942-a03f-4524aed6f31e")
    .buildRequest()
    .expand("roleDefinitionId")
    .select("principalId,action,roleDefinitionId")
    .get();

```