---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6db91f5b3f73337ac5e81e40a5df9529bc63af27
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015466"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("{school-id}").users("{user-id}")
    .buildRequest()
    .delete();

```