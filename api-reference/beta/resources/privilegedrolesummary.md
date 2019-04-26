---
title: Тип ресурса Привилежедролесуммари
description: Сводка статистики для определенной роли.
localization_priority: Normal
ms.openlocfilehash: 3e7b447f63c5f8545021508ae2dc137bef845210
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344290"
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
|Елеватедкаунт|int32|Число пользователей с назначенной ролью и активацией роли.|
|id|строка| Уникальный идентификатор для роли. Только для чтения.|
|Манажедкаунт|int32|Количество пользователей, которым назначена роль, но отключена роль.|
|Мфаенаблед|boolean|**значение true** , если для активации роли требуется mfa. **false** , если для активации роли не требуется mfa.|
|status|string| Возможные значения: `ok`, `bad`. Значение зависит от коэффициента (Манажедкаунт/Усерскаунт). Если отношение меньше заданного порогового значения, `ok` возвращается. `bad` В противном случае возвращается.|
|Усерскаунт|int32|Число пользователей, которым назначена роль.|

## <a name="relationships"></a>Связи
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
  "suppressions": []
}
-->
