---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8bebde034e9513b58d9e23d16990889aaa7969ce
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861361"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "embed";

graphClient.me().drive().items("{item-id}")
    .createLink(type,scope,expirationDateTime,password,message,recipientsList)
    .buildRequest()
    .post();

```