---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b91162e093c262feb062db6d6bebd98d169c6ca9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970642"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantPolicy permissionGrantPolicy = graphClient.policies().permissionGrantPolicies("microsoft-user-default-low")
    .buildRequest()
    .get();

```