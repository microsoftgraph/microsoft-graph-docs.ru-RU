---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b81f202509839b6f6a09120b108022a403606ce2
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212241"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChannelCollectionWithReferencesPage incomingChannels = graphClient.teams("893075dd-2487-4122-925f-022c42e20265").incomingChannels()
    .buildRequest()
    .get();

```