---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 40dd582fa90dd9dbc3541efd8dab9f0dad93c2bf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978884"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemEmail itemEmail = graphClient.users("{userId}").profile().emails("{id}")
    .buildRequest()
    .get();

```