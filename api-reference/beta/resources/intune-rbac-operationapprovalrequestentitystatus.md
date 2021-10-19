---
title: тип ресурса operationApprovalRequestEntityStatus
description: Объект OperationApprovalRequestEntityStatus
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cef153334cdd30044a75ed1cc0e322f6e94ecb64
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60487913"
---
# <a name="operationapprovalrequestentitystatus-resource-type"></a>тип ресурса operationApprovalRequestEntityStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект OperationApprovalRequestEntityStatus

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|requestId|String|ID operationApprovalRequest для этого объекта. Это свойство доступно только для чтения.|
|requestExpirationDateTime|DateTimeOffset|DateTime, в котором действия по запросу больше не разрешены. Это свойство доступно только для чтения.|
|requestStatus|[operationApprovalRequestStatus](../resources/intune-rbac-operationapprovalrequeststatus.md)|Текущий статус запроса на утверждение. Это свойство доступно только для чтения. Возможные значения: `unknown`, `needsApproval`, `approved`, `rejected`, `cancelled`, `completed`, `expired`.|
|entityLocked|Логический|Состояние объекта в отношении изменений, разрешенных дальнейших запросов или блокировки объекта. Это свойство доступно только для чтения.|

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



