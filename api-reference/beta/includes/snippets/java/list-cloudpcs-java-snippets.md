---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1b450c47e47cb88d2145f2ffcfa06dc5e9d5839545603eaadabbb42dfd30260b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57054861"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPCCollectionPage cloudPCs = graphClient.deviceManagement().virtualEndpoint().cloudPCs()
    .buildRequest()
    .get();

```