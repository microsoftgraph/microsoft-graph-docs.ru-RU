---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 61fe492d9a34e2e741df432dbe8384c3a9ea18a4
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474742"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RbacApplicationRoleScheduleInstancesCollectionPage roleScheduleInstances = graphClient.roleManagement().directory()
    .roleScheduleInstances(RbacApplicationRoleScheduleInstancesParameterSet
        .newBuilder()
        .withDirectoryScopeId("parameterValue")
        .withAppScopeId("parameterValue")
        .withPrincipalId("parameterValue")
        .withRoleDefinitionId("parameterValue")
        .build())
    .buildRequest()
    .get();

```