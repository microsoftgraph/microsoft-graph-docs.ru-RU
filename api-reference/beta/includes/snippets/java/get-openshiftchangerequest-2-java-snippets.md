---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d50d066e2c2d0fd61cbaf6d48f6ee11a97aef5f0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954360"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOpenShiftChangeRequestCollectionPage openShiftChangeRequests = graphClient.teams("{id}").schedule().openShiftChangeRequests()
    .buildRequest()
    .get();

```