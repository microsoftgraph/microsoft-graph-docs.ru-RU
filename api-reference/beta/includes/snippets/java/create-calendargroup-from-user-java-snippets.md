---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dc7145732fae6f94cfe4095fc54a493a2386692e
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507797"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarGroup calendarGroup = new CalendarGroup();
calendarGroup.name = "Personal events";

graphClient.me().calendarGroups()
    .buildRequest()
    .post(calendarGroup);

```