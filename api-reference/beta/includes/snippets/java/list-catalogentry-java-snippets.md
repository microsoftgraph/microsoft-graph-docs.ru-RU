---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 954712e7f626bc36ba4be474889b9440c2e9e4257fb21cf2de43d4bc65342ea3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57255427"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CatalogEntryCollectionPage entries = graphClient.admin().windows().updates().catalog().entries()
    .buildRequest()
    .get();

```