---
title: Тип ресурса privilegedRoleSummary
description: Сводка статистики для определенной роли.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: c8917786bfce56910555e2ea5aea98dfd0af3a75
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397502"
---
# <a name="privilegedrolesummary-resource-type"></a>Тип ресурса privilegedRoleSummary

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сводка статистики для определенной роли.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |Чтение свойств и связей объекта privilegedRoleSummary.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|elevatedCount|int32|Число пользователей, которым назначена роль и роль активирована.|
|id|string| Уникальный идентификатор роли. Только для чтения.|
|managedCount|int32|Количество пользователей, которым назначена роль, но роль отключена.|
|mfaEnabled|логический|`true` , если для активации роли требуется многофакторная проверка подлинности. `false` if the role activation doesn't require MFA.|
|status|roleSummaryStatus| Возможные значения: `ok`, `bad`. Значение зависит от соотношения (managedCount /usersCount). Если коэффициент меньше предопределенного порогового значения, `ok` возвращается. В противном `bad` случае возвращается.|
|usersCount|int32|Количество пользователей, которым назначена роль.|

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


