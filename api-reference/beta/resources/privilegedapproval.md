---
title: Тип ресурса privilegedApproval
description: Представляет утверждения, запрашиваемых в привилегированной управления удостоверениями для получения в роли.
localization_priority: Normal
ms.openlocfilehash: 03cdba4eee7b031645928b2f512288a18ba18bf8
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571019"
---
# <a name="privilegedapproval-resource-type"></a>Тип ресурса privilegedApproval

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|approvalDuration|Длительность||
|approvalState|string| Возможные значения: `pending`, `approved`, `denied`, `aborted`, `canceled`.|
|approvalType|Строка||
|approverReason|Строка||
|endDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|Строка| Только для чтения.|
|requestorReason|Строка||
|roleId|Строка||
|startDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|userId|String||

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|roleInfo| [privilegedRole](privilegedrole.md) | Только для чтения. Допускается значение null.|
|запрос| [privilegedRoleAssignmentRequest](privilegedroleassignmentrequest.md) | Только для чтения. Запрос назначения ролей для данного объекта утверждения|

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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedapproval.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
