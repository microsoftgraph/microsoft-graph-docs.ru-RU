---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4e7ac0f74bc2eee511d71444e071731d7579f430
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513634"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSettingTemplate groupSettingTemplate = graphClient.groupSettingTemplates("08d542b9-071f-4e16-94b0-74abb372e3d9")
    .buildRequest()
    .get();

```