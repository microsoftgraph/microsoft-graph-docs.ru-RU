---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 83dede3ef309c3f342b1dd9182a183b2d019aa0153b4d56334fc5500e79a4ac7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57269645"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartCollectionPage charts = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts()
    .buildRequest()
    .get();

```