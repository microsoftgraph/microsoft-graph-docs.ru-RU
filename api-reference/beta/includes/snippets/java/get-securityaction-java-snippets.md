---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b88fb8eff0d16b750f49876ea54937c4c597e838ca7c16f462755e1cac8d75c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57263419"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecurityAction securityAction = graphClient.security().securityActions("{id}")
    .buildRequest()
    .get();

```