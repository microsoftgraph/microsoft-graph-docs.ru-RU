---
title: тип ресурса privilegedApproval
description: Представляет утверждение, запрашиваемого в привилегированном управлении удостоверениями для получения роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8d092d6c877f9fa2bdce2d645ef56a84508c510d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962590"
---
# <a name="privilegedapproval-resource-type"></a>тип ресурса privilegedApproval

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет утверждение, запрашиваемого в привилегированном управлении удостоверениями для получения роли.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение privilegedApproval](../api/privilegedapproval-get.md) | [privilegedApproval](privilegedapproval.md) |Чтение свойств и связей объекта privilegedApproval.|
|[Список объектов privilegedApproval](../api/privilegedapproval-list.md) | Коллекция [privilegedApproval](privilegedapproval.md)|Получите коллекцию privilegedApproval.|
|[Создание privilegedApproval](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |Создание объекта privilegedApproval. |
|[Обновление privilegedApproval](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |Обновление объекта privilegedApproval. |
|[Myrequests](../api/privilegedapproval-myrequests.md)|[privilegedApproval](privilegedapproval.md)|Получение запросов утверждения запрашивающей стороны.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|approvalDuration|Duration||
|approvalState|approvalState| Возможные значения: `pending`, `approved`, `denied`, `aborted`, `canceled`.|
|approvalType|Строка||
|approverReason|Строка||
|endDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|String| Только для чтения.|
|requestorReason|Строка||
|roleId|Строка||
|startDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|userId|String||

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| Только для чтения. Допускается значение null.|
|запрос|[privilegedRoleAssignmentRequest](privilegedroleassignmentrequest.md)| Только для чтения. Запрос назначения ролей для этого объекта утверждения|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedApproval"
}-->

```json
{
  "approvalDuration": "string (timestamp)",
  "approvalState": "string",
  "approvalType": "string",
  "approverReason": "String",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "requestorReason": "String",
  "roleId": "String",
  "startDateTime": "String (timestamp)",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


