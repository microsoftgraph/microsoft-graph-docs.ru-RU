---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aba6080082788d6052210c6e34e247280600392a010ce79f060b38568635244a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57053964"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterCapabilities printerCapabilities = graphClient.print().printers("{id}")
    .getCapabilities()
    .buildRequest()
    .get();

```