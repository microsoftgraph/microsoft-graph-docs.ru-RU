---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6d0697df4778e52b31f2e22024772ea59ddd95dda6f85f5f4faba5c7bf607cae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57371431"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdatableAssetCollectionPage updatableAssets = graphClient.admin().windows().updates().updatableAssets()
    .buildRequest()
    .filter("isof('microsoft.graph.windowsUpdates.azureADDevice')")
    .get();

```