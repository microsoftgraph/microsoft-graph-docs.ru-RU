---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 26f2a024d780ebb6fca236f10a048bd671fb53d2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972075"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.chats("19:ea28e88c00e94c7786b065394a61f296@thread.v2").tabs("d731fca0-0f14-4537-971a-0ef9101ff13d")
    .buildRequest()
    .delete();

```