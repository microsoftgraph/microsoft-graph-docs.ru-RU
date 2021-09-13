---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9bd0681baf84ecc0945d9b93d0948afb7567eee4fddd66d50cf4c46103154387
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57307751"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartPointCollectionPage points = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series("{series-id}").points()
    .buildRequest()
    .get();

```