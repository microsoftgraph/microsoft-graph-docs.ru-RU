---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0617285aca3285238ad814c511874b6c81bf1e9e
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524297"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPermissionGrantPolicyCollectionPage permissionGrantPolicies = graphClient.policies().permissionGrantPolicies()
    .buildRequest()
    .get();

```