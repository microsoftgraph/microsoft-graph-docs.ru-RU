---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4db63f2b9840ee6d6cf3da8510594aa68ec7a02507d0c534eef271498101f3a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140304"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanDetails plannerPlanDetails = graphClient.planner().plans("{plan-id}").details()
    .buildRequest()
    .get();

```