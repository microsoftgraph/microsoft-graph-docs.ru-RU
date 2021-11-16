---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: efba0ec0391c28be7da0ff612911b3312d34cd25466627a60ae0edea33b419dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57307085"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConditionalAccessPolicyCoverageCollectionPage conditionalAccessPolicyCoverages = graphClient.tenantRelationships().managedTenants().conditionalAccessPolicyCoverages()
    .buildRequest()
    .get();

```