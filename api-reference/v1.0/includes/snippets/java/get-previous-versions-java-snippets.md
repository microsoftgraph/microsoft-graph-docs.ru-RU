---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 33b054e00fbf8b6051a565a133690d68785c46ead22b7850c618b45d2af8d008
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050359"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemVersionCollectionPage versions = graphClient.me().drive().items("{item-id}").versions()
    .buildRequest()
    .get();

```