---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 15ab5053492e993f6eb2ac2faa51c78f88e6aeac4b19d057c10b34fbecbf8013
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57192119"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagementIntentCollectionPage managementIntents = graphClient.tenantRelationships().managedTenants().managementIntents()
    .buildRequest()
    .get();

```