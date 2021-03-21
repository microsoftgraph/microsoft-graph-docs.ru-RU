---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 395e7297316b7347fec3f2e958c3c00f4eae7c72
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954283"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintUsageByPrinterCollectionPage monthlyPrintUsageSummariesByPrinter = graphClient.print().reports().monthlyPrintUsageSummariesByPrinter()
    .buildRequest()
    .get();

```