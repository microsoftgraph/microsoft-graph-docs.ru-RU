---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 90b0e8ba3456093a80cfc37140605a4c8ed7b48948105260ed7a250b60a0e9f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57192089"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantDetailedInformationCollectionPage tenantsDetailedInformation = graphClient.tenantRelationships().managedTenants().tenantsDetailedInformation()
    .buildRequest()
    .get();

```