---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 26a0eab7fb0872b13d7e43f63a84ab6a003a8d95705de43c3de116f0eb29e193
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57368511"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdatableAssetGroup updatableAsset = new UpdatableAssetGroup();

graphClient.admin().windows().updates().updatableAssets()
    .buildRequest()
    .post(updatableAsset);

```