---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1ccf97312788b42a742b79878978bb51accaa18b866a25f1b61753340cb98862
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57199583"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DelegatedPermissionClassification delegatedPermissionClassification = new DelegatedPermissionClassification();
delegatedPermissionClassification.permissionId = "e1fe6dd8-ba31-4d61-89e7-88639da4683d";
delegatedPermissionClassification.permissionName = "User.Read";
delegatedPermissionClassification.classification = PermissionClassificationType.LOW;

graphClient.servicePrincipals("{id}").delegatedPermissionClassifications()
    .buildRequest()
    .post(delegatedPermissionClassification);

```