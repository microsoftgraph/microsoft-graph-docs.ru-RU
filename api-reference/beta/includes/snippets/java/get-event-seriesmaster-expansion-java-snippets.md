---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ddf554579c8d7d1b7b6eeae6337e00d0390d4bbe
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336146"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = graphClient.me().events("AAMkADAGAADDdm4NAAA=")
    .buildRequest()
    .expand("exceptionOccurrences,cancelledOccurrences")
    .select("subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences")
    .get();

```