---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 766c4379e95f8d3dbb0c98ddc4d4d896d2bbd243
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948827"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintUsageByPrinterCollectionPage dailyPrintUsageByPrinter = graphClient.reports().dailyPrintUsageByPrinter()
    .buildRequest()
    .get();

```