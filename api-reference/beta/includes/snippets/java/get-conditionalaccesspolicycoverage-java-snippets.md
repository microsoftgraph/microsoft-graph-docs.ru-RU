---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c96ec1252ff0ba6e53464f241ca3f1f7f10962b11a671029185c891006c36df5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271578"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConditionalAccessPolicyCoverage conditionalAccessPolicyCoverage = graphClient.tenantRelationships().managedTenants().conditionalAccessPolicyCoverages("{conditionalAccessPolicyCoverageId}")
    .buildRequest()
    .get();

```