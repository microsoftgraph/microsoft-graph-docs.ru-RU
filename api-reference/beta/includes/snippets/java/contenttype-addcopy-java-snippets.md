---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dbf6ceb4ef3f17729cd72ab29d89d737512e8718
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771171"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String contentType = "https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101";

graphClient.sites("id").lists("{list-id}").contentTypes()
    .addCopy(contentType)
    .buildRequest()
    .post();

```