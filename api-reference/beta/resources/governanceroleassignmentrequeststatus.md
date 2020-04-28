---
title: Тип ресурса Говернанцеролеассигнментрекуестстатус
description: Представляет состояние governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 287f9f6ab7b1442ebdd517edbb27175fc36e6108
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497407"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>Тип ресурса Говернанцеролеассигнментрекуестстатус

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).


## <a name="properties"></a>Свойства
Свойство       | Тип |Описание|
|:----|:-------------|:-----|
|status |String| Состояние запроса на назначение роли. Значение может быть `InProgress` или `Closed`.|
|подсостояние |String| Дочерний статус запроса на назначение роли. Возможные значения `Accepted`:, `PendingEvaluation` `Granted` `Denied` `PendingProvisioning` `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` `FailedAsResourceIsLocked` `ProvisioningStarted`,,,,,,,,,,,,,, и. `Provisioned` `PendingRevocation` `Revoked` `Canceled` `Failed` `PendingApprovalProvisioning` `PendingApproval`|
|статусдетаилс       |Коллекция [keyValue](../resources/keyvalue.md)| Сведения о состоянии запроса на назначение роли. Он представляет результаты оценки различных правил. |

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
