---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 44fa65af1ac0b735a12adfeffdc478ecb418cf64
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629381"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcSnapshotGetStorageAccountsCollectionPage getStorageAccounts = graphClient.deviceManagement().virtualEndpoint().snapshots()
    .getStorageAccounts(CloudPcSnapshotGetStorageAccountsParameterSet
        .newBuilder()
        .withSubscriptionId("cb6ad4c4-8a17-4245-a644-e4436b1ee204")
        .build())
    .buildRequest()
    .get();

```