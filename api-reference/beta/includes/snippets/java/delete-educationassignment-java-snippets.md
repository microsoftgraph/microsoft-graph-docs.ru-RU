---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b17de52e2fa67a7bef5fbf0f134a3ecef7001c3b
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944777"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11014").assignments("19002")
    .buildRequest()
    .delete();

```