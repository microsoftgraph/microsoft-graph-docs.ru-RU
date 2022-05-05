---
title: Тип ресурса operationApprovalRequest
description: Сущность OperationApprovalRequest
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da330c06f770e099f190dc2faa127dacc166e19a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210425"
---
# <a name="operationapprovalrequest-resource-type"></a>Тип ресурса operationApprovalRequest

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность OperationApprovalRequest

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление operationApprovalRequests](../api/intune-rbac-operationapprovalrequest-list.md)|[Коллекция operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Список свойств и связей объектов [operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) .|
|[Получение operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-get.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Чтение свойств и связей объекта [operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) .|
|[Создание operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-create.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Создайте объект [operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) .|
|[Удаление operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-delete.md)|Нет|Удаляет [operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md).|
|[Обновление operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-update.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Обновление свойств объекта [operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) .|
|[Утверждение действия](../api/intune-rbac-operationapprovalrequest-approve.md)|Строка|Утверждает запрашиваемый экземпляр operationApprovalRequest.|
|[Отклонение действия](../api/intune-rbac-operationapprovalrequest-reject.md)|Строка|Отклоняет запрашиваемый экземпляр operationApprovalRequest.|
|[Действие cancelApproval](../api/intune-rbac-operationapprovalrequest-cancelapproval.md)|Строка|Отменяет уже утвержденный экземпляр operationApprovalRequest.|
|[Действие getRequestStatus](../api/intune-rbac-operationapprovalrequest-getrequeststatus.md)|[operationApprovalRequestEntityStatus](../resources/intune-rbac-operationapprovalrequestentitystatus.md)|Пока не задокументировано.|
|[Функция getMyRequestById](../api/intune-rbac-operationapprovalrequest-getmyrequestbyid.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Пока не задокументировано.|
|[Функция getMyRequests](../api/intune-rbac-operationapprovalrequest-getmyrequests.md)|[Коллекция operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Пока не задокументировано.|
|[Действие cancelMyRequest](../api/intune-rbac-operationapprovalrequest-cancelmyrequest.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор сущности|
|requestDateTime|DateTimeOffset|DateTime запроса. Это свойство доступно только для чтения.|
|expirationDateTime|DateTimeOffset|Дата и время, когда действия по запросу больше не разрешены. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения. Это свойство доступно только для чтения.|
|Запрашивающего|[identitySet](../resources/intune-rbac-identityset.md)|Удостоверение запрашиваемого объекта. Это свойство доступно только для чтения.|
|Утверждающий|[identitySet](../resources/intune-rbac-identityset.md)|Удостоверение утверждающего. Это свойство доступно только для чтения.|
|status|[operationApprovalRequestStatus](../resources/intune-rbac-operationapprovalrequeststatus.md)|Текущее состояние запроса на утверждение. Это свойство доступно только для чтения. Возможные значения: `unknown`, `needsApproval`, `approved`, `rejected`, `cancelled`, `completed`, `expired`, `unknownFutureValue`.|
|requestJustification|Строка|Обоснование запроса. Это свойство доступно только для чтения.|
|approvalJustification|Строка|Обоснование утверждения запроса. Это свойство доступно только для чтения.|
|operationApprovalPolicies|Строка|Политики рабочего утверждения, используемые в запросе. Это свойство доступно только для чтения.|

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
  "approvalJustification": "String",
  "operationApprovalPolicies": "String"
}
```




