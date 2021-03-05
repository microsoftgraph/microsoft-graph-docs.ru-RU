---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4033b6369b280b5a7827eeae9f42c3c9c40a6830
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473922"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISessionCollectionPage sessions = graphClient.communications().callRecords("{id}").sessions()
    .buildRequest()
    .expand("segments")
    .get();

```