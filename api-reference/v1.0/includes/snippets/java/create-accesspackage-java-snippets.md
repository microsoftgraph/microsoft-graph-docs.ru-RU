---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bc94073508eb4a65459c92d91ddd887a02cc0747
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61341839"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackage accessPackage = new AccessPackage();
accessPackage.displayName = "sales reps";
accessPackage.description = "outside sales representatives";
accessPackage.isHidden = false;
AccessPackageCatalog catalog = new AccessPackageCatalog();
catalog.id = "66584aae-98bb-48cc-9458-7bee5d2a6577";
accessPackage.catalog = catalog;

graphClient.identityGovernance().entitlementManagement().accessPackages()
    .buildRequest()
    .post(accessPackage);

```