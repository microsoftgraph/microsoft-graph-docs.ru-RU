---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e30d54fdaf29d2a2f34a67514853a29ab7b7135f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959596"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintUsageByPrinterCollectionPage monthlyPrintUsageByPrinter = graphClient.reports().monthlyPrintUsageByPrinter()
    .buildRequest()
    .get();

```