---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: efad05332db56cbea138f330f4f56758b36b7db8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973731"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTable workbookTable = new WorkbookTable();
workbookTable.name = "name-value";
workbookTable.showHeaders = true;
workbookTable.showTotals = true;
workbookTable.style = "style-value";

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .buildRequest()
    .patch(workbookTable);

```