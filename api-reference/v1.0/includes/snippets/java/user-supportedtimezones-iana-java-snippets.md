---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7eba209a68259f11fa687532efdf2d3568d6ac5635a38afcd2ac9c19d30ed334
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57263146"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookUserSupportedTimeZonesCollectionPage supportedTimeZones = graphClient.me().outlook()
    .supportedTimeZones(OutlookUserSupportedTimeZonesParameterSet
        .newBuilder()
        .withTimeZoneStandard(microsoft.graph.timeZoneStandard'Iana')
        .build())
    .buildRequest()
    .get();

```