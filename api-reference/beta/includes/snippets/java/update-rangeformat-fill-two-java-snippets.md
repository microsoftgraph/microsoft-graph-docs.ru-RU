---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: da49f1db0d01466450221f382aa6388f657ccba8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967876"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#00FF00";

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("$B$1")
        .build()).format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```