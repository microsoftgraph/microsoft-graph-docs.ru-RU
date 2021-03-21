---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 689df54e5aca6636e0746ca514112cd571619750
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983145"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.italic = true;
workbookRangeFont.size = 26d;

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("$B$1")
        .build()).format().font()
    .buildRequest()
    .patch(workbookRangeFont);

```