---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 47137a3d9b6d17df644a2c9c9fb9777f1e5a8ae5ae96d2d957a6a376fdd40333
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57206752"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrgContact orgContact = graphClient.contacts("{id}")
    .buildRequest()
    .get();

```