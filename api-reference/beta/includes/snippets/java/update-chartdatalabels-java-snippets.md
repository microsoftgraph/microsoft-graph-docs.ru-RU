---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5e00897fe6f8e7dd3c242954d74a550f81b04daa
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972413"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartDataLabels workbookChartDataLabels = new WorkbookChartDataLabels();
workbookChartDataLabels.position = "position-value";
workbookChartDataLabels.showValue = true;
workbookChartDataLabels.showSeriesName = true;
workbookChartDataLabels.showCategoryName = true;
workbookChartDataLabels.showLegendKey = true;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").dataLabels()
    .buildRequest()
    .patch(workbookChartDataLabels);

```