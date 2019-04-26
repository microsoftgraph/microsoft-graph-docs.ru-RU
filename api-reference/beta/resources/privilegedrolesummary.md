---
title: Тип ресурса Привилежедролесуммари
description: Сводка статистики для определенной роли.
localization_priority: Normal
ms.openlocfilehash: 2ed34f556f52c41729bfa108fbb6eb0c608f6b67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563436"
---
# <a name="privilegedrolesummary-resource-type"></a>Тип ресурса Привилежедролесуммари

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сводка статистики для определенной роли.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |Чтение свойств и связей объекта Привилежедролесуммари.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Елеватедкаунт|Int32|Число пользователей с назначенной ролью и активацией роли.|
|id|string| Уникальный идентификатор для роли. Только для чтения.|
|Манажедкаунт|Int32|Количество пользователей, которым назначена роль, но отключена роль.|
|Мфаенаблед|boolean|**значение true** , если для активации роли требуется mfa. **false** , если для активации роли не требуется mfa.|
|status|string| Возможные значения: `ok`, `bad`. Значение зависит от коэффициента (Манажедкаунт/Усерскаунт). Если отношение меньше заданного порогового значения, `ok` возвращается. `bad` В противном случае возвращается.|
|Усерскаунт|Int32|Число пользователей, которым назначена роль.|

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
