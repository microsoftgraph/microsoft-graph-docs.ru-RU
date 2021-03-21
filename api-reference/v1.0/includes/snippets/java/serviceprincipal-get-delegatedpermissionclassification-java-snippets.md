---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c04560085b56855d6c5aa8c03610872280b38796
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967191"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DelegatedPermissionClassificationCollectionPage delegatedPermissionClassifications = graphClient.servicePrincipals("{id}").delegatedPermissionClassifications()
    .buildRequest()
    .get();

```