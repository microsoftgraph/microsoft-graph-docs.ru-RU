---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5011553cd5ce1f3ac58da8761f6443120fe78581
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753200"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<DriveRecipient> granteesList = new LinkedList<DriveRecipient>();
DriveRecipient grantees = new DriveRecipient();
grantees.email = "ryan@contoso.com";

granteesList.add(grantees);

graphClient.me().drive().items("{item-id}").permissions("{perm-id}")
    .revokeGrants(granteesList)
    .buildRequest()
    .post();

```