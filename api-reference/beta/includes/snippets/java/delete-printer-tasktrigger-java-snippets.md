---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4af2d77115d029697691428389136786e6041d229cfd1ffa73064a0b844aa6f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57196202"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("1a5f91a7-9bd1-4d5f-bb86-f43554cac51c").taskTriggers("25be207e-1154-491f-aa68-a9f7007d4bec")
    .buildRequest()
    .delete();

```