---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8eee6bb787342d569093ee481045808c880b3193
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347454"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkDeviceActivity teamworkDeviceActivity = graphClient.teamwork().devices("1ae3fe60-fe60-1ae3-60fe-e31a60fee31a").activity()
    .buildRequest()
    .get();

```