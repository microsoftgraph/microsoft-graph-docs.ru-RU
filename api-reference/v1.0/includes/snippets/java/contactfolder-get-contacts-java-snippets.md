---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7c3ef2aa22e337443fa81c53a91d94a6dfa164198cc073066cebec6abefbb938
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57371087"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactCollectionPage contacts = graphClient.me().contactFolders("{id}").contacts()
    .buildRequest()
    .get();

```