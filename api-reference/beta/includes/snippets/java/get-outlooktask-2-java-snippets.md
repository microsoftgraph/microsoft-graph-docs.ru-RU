---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e0e7c7da165658367276b0302dda5f1d780fe037
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957639"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Pacific Standard Time\""));

OutlookTask outlookTask = graphClient.me().outlook().tasks("AAMkADA1MHgwAAA=")
    .buildRequest( requestOptions )
    .get();

```