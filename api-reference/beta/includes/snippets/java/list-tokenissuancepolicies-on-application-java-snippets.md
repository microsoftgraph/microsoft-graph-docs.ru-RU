---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9bed75c4e3c06e64e0d5f8ef72fb52a04ace178c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962066"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITokenIssuancePolicyCollectionWithReferencesPage tokenIssuancePolicies = graphClient.applications("{id}").tokenIssuancePolicies()
    .buildRequest()
    .get();

```