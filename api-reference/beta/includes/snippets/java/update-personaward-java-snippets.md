---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 62d1bbf00a8786077cf4d13cd1ee045b65ccf67b668717639ae595f2eac36857
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57308040"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAward personAward = new PersonAward();
personAward.issuingAuthority = "International Association of Branding Management";
personAward.thumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg";

graphClient.users("{userId}").profile().awards("{personAwardId}")
    .buildRequest()
    .patch(personAward);

```