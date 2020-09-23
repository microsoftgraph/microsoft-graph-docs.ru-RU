---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 37893e69d08d73e7ac94cf423649f2b4f77dc168
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48222865"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.communications().calls("{id}").participants("{id}")
    .buildRequest()
    .delete();

```