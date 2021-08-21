---
title: тип ресурса governanceRoleAssignmentRequestStatus
description: Представляет состояние governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: 80994db594c2f0e45dfe36a5fbf32260266a0536
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453543"
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


