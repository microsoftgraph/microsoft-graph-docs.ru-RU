---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 624be23008d719504dd271d563382a47e929efd77a8a0b7f8d53e74fb584654b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57367418"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.onPremisesPublishingProfiles("provisioning").agentGroups("8832388F-3814-4952-B288-FFB62081FE25")
    .buildRequest()
    .delete();

```