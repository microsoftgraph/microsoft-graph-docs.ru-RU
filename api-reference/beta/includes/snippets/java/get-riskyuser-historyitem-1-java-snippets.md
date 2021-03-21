---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 63b02eb56ff643f34d88ceba91a61fceadbcf5d3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962268"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyUserHistoryItem riskyUserHistoryItem = graphClient.riskyUsers("41a31b00-3b3b-42d9-8f1c-6d4f14e74c69").history("41a31b00-3b3b-42d9-8f1c-6d4f14e74c69")
    .buildRequest()
    .get();

```