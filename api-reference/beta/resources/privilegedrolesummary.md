---
title: Тип ресурса privilegedRoleSummary
description: Сводка статистики для определенной роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 368ed2ba6b206ba102f821ceac38de70494f8718
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133976"
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
|elevatedCount|int32|Количество пользователей, для пользователей с назначенной ролью и ролью активируется.|
|id|string| Уникальный идентификатор роли. Только для чтения.|
|managedCount|int32|Количество пользователей с назначенной ролью, но отключаемой ролью.|
|mfaEnabled|boolean|**true,** если для активации роли требуется многофаксная активация. **false,** если активация роли не требует многофаксической активации.|
|status|string| Возможные значения: `ok`, `bad`. Значение зависит от соотношения (managedCount / usersCount). Если коэффициент меньше предварительно заранее установленного порогового значения, `ok` возвращается. В `bad` противном случае возвращается.|
|usersCount|int32|Количество пользователей, которые назначены этой роли.|

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


