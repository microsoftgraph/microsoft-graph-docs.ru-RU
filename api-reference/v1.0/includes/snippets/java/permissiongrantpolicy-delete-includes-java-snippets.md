---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 185d5c0511d924e7ccdd1bc4b2035ea7d771fd2da11d05c4e8f785dd9f4f7607
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57255774"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().permissionGrantPolicies("my-custom-consent-policy").includes("198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5")
    .buildRequest()
    .delete();

```