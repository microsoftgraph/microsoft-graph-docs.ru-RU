---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 71cde89c290d75ce5f42a6ac27728a88e7b16452506c3b213c04947526568a45
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57364730"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantGroup tenantGroup = graphClient.tenantRelationships().managedTenants().tenantGroups("{tenantGroupId}")
    .buildRequest()
    .get();

```