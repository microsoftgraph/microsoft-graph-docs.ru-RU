---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2ca1f5c628ea95113d88dd6fa892ab63dd57cebb
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093649"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUsageRightCollectionPage usageRights = graphClient.users("{userId}").usageRights()
    .buildRequest()
    .filter("state in ('active', 'suspended') and serviceIdentifier in ('ABCD')")
    .get();

```