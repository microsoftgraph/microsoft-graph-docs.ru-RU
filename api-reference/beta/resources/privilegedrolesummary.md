---
title: Тип ресурса Привилежедролесуммари
description: Сводка статистики для определенной роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 05b8646090726570ed0d4ec9f38862a404bbc6d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070501"
---
# <a name="privilegedrolesummary-resource-type"></a>Тип ресурса Привилежедролесуммари

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сводка статистики для определенной роли.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |Чтение свойств и связей объекта Привилежедролесуммари.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|елеватедкаунт|int32|Число пользователей с назначенной ролью и активацией роли.|
|id|string| Уникальный идентификатор для роли. Только для чтения.|
|манажедкаунт|int32|Количество пользователей, которым назначена роль, но отключена роль.|
|мфаенаблед|boolean|**значение true** , если для активации роли требуется mfa. **false** , если для активации роли не требуется mfa.|
|status|string| Возможные значения: `ok`, `bad`. Значение зависит от коэффициента (Манажедкаунт/Усерскаунт). Если отношение меньше заданного порогового значения, `ok` возвращается. В противном случае `bad` возвращается.|
|усерскаунт|int32|Число пользователей, которым назначена роль.|

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
  "suppressions": []
}
-->


