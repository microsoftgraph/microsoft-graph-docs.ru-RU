---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8f2d1a2b2b0f4ac5d58e032299c664342ca8fa50
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954543"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().featureRolloutPolicies("df85e4d9-e8c4-4033-a41c-73419a95c29c").appliesTo("2441b489-4f12-4882-b039-8f6006bd66da").reference()
    .buildRequest()
    .delete();

```