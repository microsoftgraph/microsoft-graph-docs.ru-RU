---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 744cf35fe028f9f3ea8329296a2496356113244b
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440260"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentSchedule unifiedRoleAssignmentSchedule = graphClient.roleManagement().directory().roleAssignmentSchedules("b1477448-2cc6-4ceb-93b4-54a202a89413")
    .buildRequest()
    .get();

```