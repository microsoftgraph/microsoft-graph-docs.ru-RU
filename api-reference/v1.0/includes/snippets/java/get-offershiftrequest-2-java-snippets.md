---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 671540cc182194128c2ac3489d6558cb99464505
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208211"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OfferShiftRequestCollectionPage offerShiftRequests = graphClient.teams("{teamId}").schedule().offerShiftRequests()
    .buildRequest()
    .get();

```