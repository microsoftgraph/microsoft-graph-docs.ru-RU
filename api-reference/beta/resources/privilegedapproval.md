---
title: Тип ресурса privilegedApproval
description: Представляет утверждения, запрашиваемых в привилегированной управления удостоверениями для получения в роли.
ms.openlocfilehash: 3f900ef4a141b2f71c303becd49789b86cefb1b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078701"
---
# <a name="privilegedapproval-resource-type"></a>Тип ресурса privilegedApproval

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет утверждения, запрашиваемых в привилегированной управления удостоверениями для получения в роли.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение privilegedApproval](../api/privilegedapproval-get.md) | [privilegedApproval](privilegedapproval.md) |Чтение свойства и связи объекта privilegedApproval.|
|[Список объектов privilegedApproval](../api/privilegedapproval-list.md) | [privilegedApproval](privilegedapproval.md) коллекции|Получите коллекцию privilegedApproval.|
|[Создание privilegedApproval](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |Создание объекта privilegedApproval. |
|[Обновление privilegedApproval](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |Обновление объекта privilegedApproval. |
|[Myrequests](../api/privilegedapproval-myrequests.md)|[privilegedApproval](privilegedapproval.md)|Получите запрашивающего запросов на утверждение.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|approvalDuration|Продолжительность||
|approvalState|string| Возможные значения: `pending`, `approved`, `denied`, `aborted`, `canceled`.|
|approvalType|String||
|approverReason|String||
|endDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String| Только для чтения.|
|requestorReason|String||
|roleId|String||
|startDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|userId|String||

## <a name="relationships"></a>Связи
| Связь | Тип   |Description|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| Только для чтения. Допускается значение null.|
|запрос|[privilegedRoleAssignmentRequest](privilegedroleassignmentrequest.md)| Только для чтения. Запрос назначения ролей для данного объекта утверждения|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->