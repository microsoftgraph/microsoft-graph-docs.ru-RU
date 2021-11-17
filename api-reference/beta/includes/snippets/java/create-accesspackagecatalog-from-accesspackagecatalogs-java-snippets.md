---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eeb24b5286e6a42e7ab68ab25c71ad0f8983b121faad3959d0f3c6956272c021
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57051271"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCatalog accessPackageCatalog = new AccessPackageCatalog();
accessPackageCatalog.displayName = "sales";
accessPackageCatalog.description = "for employees working with sales and outside sales partners";
accessPackageCatalog.isExternallyVisible = true;

graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs()
    .buildRequest()
    .post(accessPackageCatalog);

```