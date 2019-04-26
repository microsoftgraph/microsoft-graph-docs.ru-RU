---
title: Тип ресурса Привилежедаппровал
description: Представляет утверждение, запрошенное в результате привилегированного управления удостоверениями для доступа к роли.
localization_priority: Normal
ms.openlocfilehash: 754fcd9b61321db1675408172c945557e38dc0e0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344240"
---
# <a name="privilegedapproval-resource-type"></a>Тип ресурса Привилежедаппровал

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет утверждение, запрошенное в результате привилегированного управления удостоверениями для доступа к роли.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение privilegedApproval](../api/privilegedapproval-get.md) | [privilegedApproval](privilegedapproval.md) |Чтение свойств и связей объекта Привилежедаппровал.|
|[Список объектов Привилежедаппровал](../api/privilegedapproval-list.md) | Коллекция [privilegedApproval](privilegedapproval.md)|Получение коллекции Привилежедаппровал.|
|[Создание privilegedApproval](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |Создание объекта privilegedApproval. |
|[Обновление privilegedApproval](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |Обновление объекта privilegedApproval. |
|[Мирекуестс](../api/privilegedapproval-myrequests.md)|[privilegedApproval](privilegedapproval.md)|Получение запросов утверждения запрашивающей стороны.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Аппровалдуратион|Duration (Длительность)||
|Аппровалстате|string| Возможные значения: `pending`, `approved`, `denied`, `aborted`, `canceled`.|
|Аппровалтипе|String||
|Аппроверреасон|String||
|endDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String| Только для чтения.|
|Рекуесторреасон|String||
|roleId|String||
|startDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|userId|String||

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|Ролеинфо|[privilegedRole](privilegedrole.md)| Только для чтения. Допускает значение null.|
|Request|[Привилежедролеассигнментрекуест](privilegedroleassignmentrequest.md)| Только для чтения. Запрос на назначение роли для этого объекта утверждения|

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
