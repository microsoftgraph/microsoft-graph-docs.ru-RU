---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4d905b3b0face129e30c0fdf5a1ef11e02810078
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961692"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = graphClient.me().messages("AAMkADA1M-zAAA=").attachments("AAMkADA1M-CJKtzmnlcqVgqI=")
    .buildRequest()
    .expand("itemattachment/item")
    .get();

```