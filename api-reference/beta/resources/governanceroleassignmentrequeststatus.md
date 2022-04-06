---
title: тип ресурса governanceRoleAssignmentRequestStatus
description: Представляет состояние governanceRoleAssignmentRequest.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: 19eb182a450053400b66db12c0d2fe119908a992
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510206"
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
