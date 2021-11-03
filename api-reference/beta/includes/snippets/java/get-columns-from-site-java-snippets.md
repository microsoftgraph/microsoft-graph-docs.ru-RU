---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 21d5f956262fd4420fdde7294070dbf1a6d7e8c135290731d64697ea927e80b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57208569"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ColumnDefinitionCollectionPage columns = graphClient.sites("{site-id}").columns()
    .buildRequest()
    .get();

```