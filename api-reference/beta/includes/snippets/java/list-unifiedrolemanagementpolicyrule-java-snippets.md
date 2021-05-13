---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d187d52691224e3573e29afe65eabed0bab55374
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474302"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyRuleCollectionPage effectiveRules = graphClient.policies().roleManagementPolicies("ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba").effectiveRules()
    .buildRequest()
    .get();

```