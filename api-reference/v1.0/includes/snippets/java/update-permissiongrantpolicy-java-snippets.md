---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ca47dd951d34837df33038e3d5eb011013029157cc28b1dce9c4d7e6d3338624
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57316159"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantPolicy permissionGrantPolicy = new PermissionGrantPolicy();
permissionGrantPolicy.displayName = "Custom permission grant policy";

graphClient.policies().permissionGrantPolicies("my-custom-consent-policy")
    .buildRequest()
    .patch(permissionGrantPolicy);

```