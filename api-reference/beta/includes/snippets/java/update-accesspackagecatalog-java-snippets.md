---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fc5718a910b3604ffffbc71c8d4870d2e4c9e3b93f2d551a1dce1f428ffc7ff3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57051270"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCatalog accessPackageCatalog = new AccessPackageCatalog();
accessPackageCatalog.displayName = "Catalog One";

graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("{accessPackageCatalogId}")
    .buildRequest()
    .patch(accessPackageCatalog);

```