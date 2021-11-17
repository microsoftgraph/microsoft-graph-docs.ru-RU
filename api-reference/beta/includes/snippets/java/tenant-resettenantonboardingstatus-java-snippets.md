---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9d783814ecc64d0f9ccec518e8d2b9db8e8278d38bdb5603bafb3d7ed8b8e45a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57206029"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.tenantRelationships().managedTenants().tenants("{tenantId}")
    .resetTenantOnboardingStatus()
    .buildRequest()
    .post();

```