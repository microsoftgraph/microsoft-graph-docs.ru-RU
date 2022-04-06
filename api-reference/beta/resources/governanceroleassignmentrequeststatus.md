---
title: тип ресурса governanceRoleAssignmentRequestStatus
description: Представляет состояние governanceRoleAssignmentRequest.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: e023b40cd5c23c6b6f34d18c51eb7681354587b1
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723012"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>тип ресурса governanceRoleAssignmentRequestStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).

## <a name="properties"></a>Свойства

| Свойство      | Тип                                            | Описание                                                                                                                                                                                                                                                                                                                                                                                     |
| :------------ | :---------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| status        | String                                          | Состояние запроса на назначение ролей. Значение может быть или `InProgress` `Closed`.                                                                                                                                                                                                                                                                                                           |
| subStatus     | String                                          | Состояние подгруппы запроса назначения ролей. Значения могут быть , , , , , , `Provisioned`, `PendingRevocation``Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingAdminDecision``AdminApproved``FailedAsResourceIsLocked``PendingApproval`, , `AdminDenied`и .`ProvisioningStarted``TimedOut``PendingProvisioning``Denied``Granted``PendingEvaluation``Accepted` |
| statusDetails | Коллекция [keyValue](../resources/keyvalue.md) | Сведения о состоянии запроса на назначение ролей. Он представляет результаты оценки различных правил.                                                                                                                                                                                                                                                                              |

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
