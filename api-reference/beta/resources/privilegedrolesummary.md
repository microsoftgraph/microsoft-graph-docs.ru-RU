---
title: Тип ресурса Привилежедролесуммари
description: Сводка статистики для определенной роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 47ab49c6f91684924dab02d590427a875c1baa01
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521490"
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
|id|строка| Уникальный идентификатор для роли. Только для чтения.|
|манажедкаунт|int32|Количество пользователей, которым назначена роль, но отключена роль.|
|мфаенаблед|boolean|**значение true** , если для активации роли требуется mfa. **false** , если для активации роли не требуется mfa.|
|status|string| Возможные значения: `ok`, `bad`. Значение зависит от коэффициента (Манажедкаунт/Усерскаунт). Если отношение меньше заданного порогового значения, `ok` возвращается. `bad` В противном случае возвращается.|
|усерскаунт|int32|Число пользователей, которым назначена роль.|

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
