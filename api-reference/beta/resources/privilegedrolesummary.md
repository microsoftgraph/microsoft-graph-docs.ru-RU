---
title: Тип ресурса privilegedRoleSummary
description: Статистика для определенной роли.
ms.openlocfilehash: f6c66433651eff188ce6fdaa07c2422d3bb6e0ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081320"
---
# <a name="privilegedrolesummary-resource-type"></a>Тип ресурса privilegedRoleSummary

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Статистика для определенной роли.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |Чтение свойства и связи объекта privilegedRoleSummary.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|elevatedCount|int32|Число пользователей, имеющих роли, назначенной и роль активирован.|
|id|строка| Уникальный идентификатор для роли. Только для чтения.|
|managedCount|int32|Число пользователей, имеющих роли, назначенной, но роль отключена.|
|mfaEnabled|boolean|**значение true,** Если требуется для активации роли многофакторной проверкой Подлинности. **значение false,** Если роль активации не требует многофакторной проверкой Подлинности.|
|status|string| Возможные значения: `ok`, `bad`. Значение зависит от отношение числа (managedCount / usersCount). Если отношение меньше, чем пороговых, `ok` возвращается. В противном случае `bad` возвращается.|
|usersCount|int32|Число пользователей, которым назначен роли.|

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->