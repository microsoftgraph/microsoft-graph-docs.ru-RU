---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d7cc744d03fbfe0f009357709e17294ab7827e8c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131039"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DeviceCompliancePolicySettingStateSummary deviceCompliancePolicySettingStateSummary = graphClient.tenantRelationships().managedTenants().deviceCompliancePolicySettingStateSummaries("{deviceCompliancePolicySettingStateSummaryId}")
    .buildRequest()
    .get();

```