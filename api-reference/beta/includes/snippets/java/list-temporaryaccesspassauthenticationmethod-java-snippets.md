---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ef29b6095519ad9bf4c4b617788b72fca2622193b58e92574b6f3c920b413832
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57139619"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TemporaryAccessPassAuthenticationMethodCollectionPage temporaryAccessPassMethods = graphClient.me().authentication().temporaryAccessPassMethods()
    .buildRequest()
    .get();

```