---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ec7b31a704da33dcfcaae7e40f424b65a11edc58
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62138294"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantCustomizedInformation tenantCustomizedInformation = new TenantCustomizedInformation();
tenantCustomizedInformation.tenantId = "String";
LinkedList<TenantContactInformation> contactsList = new LinkedList<TenantContactInformation>();
TenantContactInformation contacts = new TenantContactInformation();
contacts.name = "String";
contacts.title = "String";
contacts.email = "String";
contacts.phone = "String";
contacts.notes = "String";
contactsList.add(contacts);
tenantCustomizedInformation.contacts = contactsList;
tenantCustomizedInformation.website = "String";

graphClient.tenantRelationships().managedTenants().tenantsCustomizedInformation("{tenantCustomizedInformationId}")
    .buildRequest()
    .patch(tenantCustomizedInformation);

```