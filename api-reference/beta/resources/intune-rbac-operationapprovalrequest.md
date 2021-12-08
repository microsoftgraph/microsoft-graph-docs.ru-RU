---
title: тип ресурса operationApprovalRequest
description: Объект OperationApprovalRequest
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 45c2b30a39c9930ee8a8d7def27a06e7617fddbf
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346747"
---
# <a name="operationapprovalrequest-resource-type"></a>тип ресурса operationApprovalRequest

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект OperationApprovalRequest

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список операцийApprovalRequests](../api/intune-rbac-operationapprovalrequest-list.md)|[коллекция operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Список свойств и связей объектов [operationApprovalRequest.](../resources/intune-rbac-operationapprovalrequest.md)|
|[Получить operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-get.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Чтение свойств и связей объекта [operationApprovalRequest.](../resources/intune-rbac-operationapprovalrequest.md)|
|[Создание operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-create.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Создание нового [объекта operationApprovalRequest.](../resources/intune-rbac-operationapprovalrequest.md)|
|[Удаление operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-delete.md)|Нет|Удаляет [операциюApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md).|
|[Обновление операцииApprovalRequest](../api/intune-rbac-operationapprovalrequest-update.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Обновление свойств объекта [operationApprovalRequest.](../resources/intune-rbac-operationapprovalrequest.md)|
|[утверждение действия](../api/intune-rbac-operationapprovalrequest-approve.md)|String|Утверждает запрошенный экземпляр операцииApprovalRequest|
|[отклонение действия](../api/intune-rbac-operationapprovalrequest-reject.md)|Строка|Отклонение запрошеного экземпляра операцииApprovalRequest|
|[cancelApproval action](../api/intune-rbac-operationapprovalrequest-cancelapproval.md)|String|Отмена уже утвержденного экземпляра операцииApprovalRequest|
|[действие getRequestStatus](../api/intune-rbac-operationapprovalrequest-getrequeststatus.md)|[operationApprovalRequestEntityStatus](../resources/intune-rbac-operationapprovalrequestentitystatus.md)|Пока не задокументировано.|
|[функция getMyRequestById](../api/intune-rbac-operationapprovalrequest-getmyrequestbyid.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Пока не задокументировано.|
|[функция getMyRequests](../api/intune-rbac-operationapprovalrequest-getmyrequests.md)|[коллекция operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Пока не задокументировано.|
|[cancelMyRequest action](../api/intune-rbac-operationapprovalrequest-cancelmyrequest.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID объекта|
|requestDateTime|DateTimeOffset|DateTime запроса. Это свойство доступно только для чтения.|
|expirationDateTime|DateTimeOffset|DateTime, в котором действия по запросу больше не разрешены. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Последнее изменение DateTime. Это свойство доступно только для чтения.|
|запросчик|[identitySet](../resources/intune-rbac-identityset.md)|Удостоверение запросителя. Это свойство доступно только для чтения.|
|одобрение|[identitySet](../resources/intune-rbac-identityset.md)|Удостоверение утвержденного. Это свойство доступно только для чтения.|
|status|[operationApprovalRequestStatus](../resources/intune-rbac-operationapprovalrequeststatus.md)|Текущий статус запроса на утверждение. Это свойство доступно только для чтения. Возможные значения: `unknown`, `needsApproval`, `approved`, `rejected`, `cancelled`, `completed`, `expired`.|
|requestJustification|Строка|Обоснование запроса. Это свойство доступно только для чтения.|
|approvalJustification|Строка|Обоснование утверждения запроса. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.operationApprovalRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operationApprovalRequest",
  "id": "String (identifier)",
  "requestDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "requestor": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    }
  },
  "approver": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    }
  },
  "status": "String",
  "requestJustification": "String",
  "approvalJustification": "String"
}
```




