---
title: тип ресурса operationApprovalRequestEntityStatus
description: Объект OperationApprovalRequestEntityStatus
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7449a0fd644e23bd7cba49398ecb3c84ac6e739d
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61343590"
---
# <a name="operationapprovalrequestentitystatus-resource-type"></a>тип ресурса operationApprovalRequestEntityStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект OperationApprovalRequestEntityStatus

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|requestId|Строка|ID operationApprovalRequest для этого объекта. Это свойство доступно только для чтения.|
|requestExpirationDateTime|DateTimeOffset|DateTime, в котором действия по запросу больше не разрешены. Это свойство доступно только для чтения.|
|requestStatus|[operationApprovalRequestStatus](../resources/intune-rbac-operationapprovalrequeststatus.md)|Текущий статус запроса на утверждение. Это свойство доступно только для чтения. Возможные значения: `unknown`, `needsApproval`, `approved`, `rejected`, `cancelled`, `completed`, `expired`.|
|entityLocked|Boolean|Состояние объекта в отношении изменений, разрешенных дальнейших запросов или блокировки объекта. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationApprovalRequestEntityStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operationApprovalRequestEntityStatus",
  "requestId": "String",
  "requestExpirationDateTime": "String (timestamp)",
  "requestStatus": "String",
  "entityLocked": true
}
```




