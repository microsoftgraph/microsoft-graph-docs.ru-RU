---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0f8eb3f7009e51138eb342ebe4d14c912b289c5908ff24f6e472e4ba48a0a49e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57053279"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagementActionTenantDeploymentStatusCollectionPage managementActionTenantDeploymentStatuses = graphClient.tenantRelationships().managedTenants().managementActionTenantDeploymentStatuses()
    .buildRequest()
    .get();

```