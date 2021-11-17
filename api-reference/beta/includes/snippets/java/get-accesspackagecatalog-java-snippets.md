---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dff2f5db1948f556e61b96265ca04c9adc80bfc5b360eb08567cc8f5de5a38e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57191237"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCatalog accessPackageCatalog = graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("{id}")
    .buildRequest()
    .get();

```