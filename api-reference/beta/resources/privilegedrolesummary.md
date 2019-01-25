---
title: Тип ресурса privilegedRoleSummary
description: Статистика для определенной роли.
localization_priority: Normal
ms.openlocfilehash: 2ed34f556f52c41729bfa108fbb6eb0c608f6b67
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513741"
---
# <a name="privilegedrolesummary-resource-type"></a>Тип ресурса privilegedRoleSummary

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Статистика для определенной роли.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |Чтение свойства и связи объекта privilegedRoleSummary.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|elevatedCount|int32|Число пользователей, имеющих роли, назначенной и роль активирован.|
|id|string| Уникальный идентификатор для роли. Только для чтения.|
|managedCount|int32|Число пользователей, имеющих роли, назначенной, но роль отключена.|
|mfaEnabled|boolean|**значение true,** Если требуется для активации роли многофакторной проверкой Подлинности. **значение false,** Если роль активации не требует многофакторной проверкой Подлинности.|
|status|string| Возможные значения: `ok`, `bad`. Значение зависит от отношение числа (managedCount / usersCount). Если отношение меньше, чем пороговых, `ok` возвращается. В противном случае `bad` возвращается.|
|usersCount|int32|Число пользователей, которым назначен роли.|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
}-->

```json
{
  "elevatedCount": 1024,
  "id": "string (identifier)",
  "managedCount": 1024,
  "mfaEnabled": true,
  "status": "string",
  "usersCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesummary.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
