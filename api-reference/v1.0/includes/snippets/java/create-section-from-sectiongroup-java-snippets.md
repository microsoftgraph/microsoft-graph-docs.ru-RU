---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 30e7a4c84ef85c9f7d716d03e4eb1c8f55e51d40
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968441"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnenoteSection onenoteSection = new OnenoteSection();
onenoteSection.displayName = "Section name";

graphClient.me().onenote().sectionGroups("{id}").sections()
    .buildRequest()
    .post(onenoteSection);

```