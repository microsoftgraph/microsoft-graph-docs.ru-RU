---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 186c5a1d9531cc390f9a0fdd94150f13a0bebe1dd0637078e4589f371b69d9e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57315341"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnenoteSection onenoteSection = new OnenoteSection();
onenoteSection.displayName = "Section name";

graphClient.me().onenote().sectionGroups("{id}").sections()
    .buildRequest()
    .post(onenoteSection);

```