---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ef045975542681c03afbfa969a4b368db85f5508
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442035"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content deviceCompliancePolicySettingStateSummary = graphClient.tenantRelationships().managedTenants().deviceCompliancePolicySettingStateSummary()
    .buildRequest()
    .get();

```