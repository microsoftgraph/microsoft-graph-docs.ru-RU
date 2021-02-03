---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a47194dc6aad91eda2a34de3abf65be3d666a776
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092341"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserRegistrationFeatureSummary userRegistrationFeatureSummary = graphClient.reports().authenticationMethods()
    .usersRegisteredByFeature('all','all')
    .buildRequest()
    .get();

```