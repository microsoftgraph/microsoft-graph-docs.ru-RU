---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 02c1c21a107535cd62a3d1f366d6dedca158af0831114558c5460d0b1c1ae269
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213200"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanCollectionWithReferencesPage rosterPlans = graphClient.users("{usersId}").planner().rosterPlans()
    .buildRequest()
    .get();

```