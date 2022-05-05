---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a6fd7d7643624f88fa292a671df3a7ffa9d3cc8b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206727"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleRequest unifiedRoleEligibilityScheduleRequest = new UnifiedRoleEligibilityScheduleRequest();
unifiedRoleEligibilityScheduleRequest.action = "adminRemove";
unifiedRoleEligibilityScheduleRequest.roleDefinitionId = "8424c6f0-a189-499e-bbd0-26c1753c96d4";
unifiedRoleEligibilityScheduleRequest.directoryScopeId = "/";
unifiedRoleEligibilityScheduleRequest.principalId = "071cc716-8147-4397-a5ba-b2105951cc0b";

graphClient.roleManagement().directory().roleEligibilityScheduleRequests()
    .buildRequest()
    .post(unifiedRoleEligibilityScheduleRequest);

```