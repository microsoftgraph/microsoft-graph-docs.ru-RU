---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 69bea8ef48f7e10b57d8591ce934780dd6e2902a1cc9b652b3cd00ecc384c537
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138612"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackage accessPackage = new AccessPackage();
accessPackage.displayName = "Access Package New Name";

graphClient.identityGovernance().entitlementManagement().accessPackages("{accessPackageId}")
    .buildRequest()
    .patch(accessPackage);

```