---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 787cc0d4e5d33b336e85fd19c43cec03391d5571942ae18e5f93b0751242fea4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57306989"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeBorderCollectionPage borders = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().borders()
    .buildRequest()
    .get();

```