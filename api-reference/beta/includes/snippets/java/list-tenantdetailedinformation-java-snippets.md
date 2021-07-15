---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5794001ed7be65912dfd3964afa956ac5f55ee06
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440603"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantDetailedInformationCollectionPage tenantsDetailedInformation = graphClient.tenantRelationships().managedTenants().tenantsDetailedInformation()
    .buildRequest()
    .get();

```