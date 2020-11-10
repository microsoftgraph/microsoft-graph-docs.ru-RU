---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1ed995a24ccbfa5cad366e6c78953de4a2d4f64d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980965"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TrustFrameworkKeySet trustFrameworkKeySet = graphClient.trustFramework().keySets("{id}")
    .buildRequest()
    .get();

```