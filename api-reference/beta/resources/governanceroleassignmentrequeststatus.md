---
title: тип ресурса governanceRoleAssignmentRequestStatus
description: Представляет состояние governanceRoleAssignmentRequest.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: e04b49fedf761ef3715d152fdc2a07a3af139bc3
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695414"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>тип ресурса governanceRoleAssignmentRequestStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).


## <a name="properties"></a>Свойства
Свойство       | Тип |Описание|
|:----|:-------------|:-----|
|status |String| Состояние запроса на назначение ролей. Значение может быть `InProgress` или `Closed` .|
|subStatus |String| Состояние подгруппы запроса назначения ролей. Значения могут быть `Accepted` `PendingEvaluation` , , , , , `Granted` , , , , , , `Denied` `PendingProvisioning` , , `Provisioned` `PendingRevocation` и `Revoked` `Canceled` `Failed` `PendingApprovalProvisioning` `PendingApproval` `FailedAsResourceIsLocked` `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` `ProvisioningStarted` .|
|statusDetails       |Коллекция [keyValue](../resources/keyvalue.md)| Сведения о состоянии запроса на назначение ролей. Он представляет результаты оценки различных правил. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"
}-->


```json
{
  "status": "String",
  "subStatus": "String",
  "statusDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequestStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


