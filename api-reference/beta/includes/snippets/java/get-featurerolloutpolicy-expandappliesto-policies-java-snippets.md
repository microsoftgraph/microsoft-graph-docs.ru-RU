---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f7398d9e87da767462ea84cccd0923da40c228e2
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508688"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FeatureRolloutPolicy featureRolloutPolicy = graphClient.policies().featureRolloutPolicies("df85e4d9-e8c4-4033-a41c-73419a95c29c")
    .buildRequest()
    .expand("appliesTo")
    .get();

```