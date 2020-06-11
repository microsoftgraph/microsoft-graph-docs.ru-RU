---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3aa1a6e680c317d55d0137e7dece9b9c45a76299
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684987"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemAttachment attachment = new ItemAttachment();
attachment.name = "name-value";
attachment.item = "{message or event entity}";

graphClient.me().events("{id}").attachments()
    .buildRequest()
    .post(attachment);

```