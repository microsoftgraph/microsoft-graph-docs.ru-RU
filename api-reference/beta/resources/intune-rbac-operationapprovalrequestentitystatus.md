---
title: Тип ресурса operationApprovalRequestEntityStatus
description: Объект OperationApprovalRequestEntityStatus
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ffc877ddf0a724b1471c55e2b9edb0455e4da0fb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209130"
---
# <a name="operationapprovalrequestentitystatus-resource-type"></a>Тип ресурса operationApprovalRequestEntityStatus

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект OperationApprovalRequestEntityStatus

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|requestId|Строка|Идентификатор OperationApprovalRequest для этой сущности. Это свойство доступно только для чтения.|
|requestExpirationDateTime|DateTimeOffset|Дата и время, когда действия по запросу больше не разрешены. Это свойство доступно только для чтения.|
|requestStatus|[operationApprovalRequestStatus](../resources/intune-rbac-operationapprovalrequeststatus.md)|Текущее состояние запроса на утверждение. Это свойство доступно только для чтения. Возможные значения: `unknown`, `needsApproval`, `approved`, `rejected`, `cancelled`, `completed`, `expired`, `unknownFutureValue`.|
|entityLocked|Логическое|Состояние сущности в отношении изменений, разрешено ли дальнейшие запросы или сущность заблокирована. Это свойство доступно только для чтения.|

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




