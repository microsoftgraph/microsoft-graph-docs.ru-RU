---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a77fc023f94ea0cd6c50736713e3ab15f21a9244
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984150"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerBucketTaskBoardTaskFormat plannerBucketTaskBoardTaskFormat = graphClient.planner().tasks("01gzSlKkIUSUl6DF_EilrmQAKDhh").bucketTaskBoardFormat()
    .buildRequest()
    .get();

```