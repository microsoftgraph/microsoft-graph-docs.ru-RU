---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 19d8fad1c12e181788113d7b16153c2e59b2bfd0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315569"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyCollectionPage roleManagementPolicies = graphClient.policies().roleManagementPolicies()
    .buildRequest()
    .filter("scopeId eq '/' and scopeType eq 'Directory'")
    .expand("rules")
    .get();

```