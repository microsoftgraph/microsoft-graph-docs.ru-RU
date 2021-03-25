---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9ed8fdc892763980669a4735be9f43ddcd6c3917
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210868"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ShiftPreferences shiftPreferences = graphClient.users("871dbd5c-3a6a-4392-bfe1-042452793a50").settings().shiftPreferences()
    .buildRequest()
    .get();

```