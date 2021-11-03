---
title: тип ресурса privilegedRoleSummary
description: Сводка статистики для определенной роли.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: e65179dcbccd6651bbfe51a314ea15a12a57da58
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694152"
---
# <a name="privilegedrolesummary-resource-type"></a>тип ресурса privilegedRoleSummary

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
|elevatedCount|int32|Число пользователей, которые имеют назначенную роль и роль активируется.|
|id|string| Уникальный идентификатор роли. Только для чтения.|
|managedCount|int32|Число пользователей, которые имеют назначенную роль, но роль отключена.|
|mfaEnabled|логический|`true` если активация роли требует MFA. `false` если активация роли не требует MFA.|
|status|roleSummaryStatus| Возможные значения: `ok`, `bad`. Значение зависит от соотношения (managedCount /usersCount). Если коэффициент меньше заранее установленного порогового значения, `ok` возвращается. В `bad` противном случае возвращается.|
|usersCount|int32|Число пользователей, которые назначены с ролью.|

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


