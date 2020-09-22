---
title: Тип ресурса Планнерфаворитепланреференце
description: 'Тип ресурса **планнерфаворитепланреференце** репесентс ссылку на plannerPlan, помеченную пользователем в качестве избранного. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e5a25f7a1e4e27ca0d0061c616f441dd8cc53cde
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979352"
---
# <a name="plannerfavoriteplanreference-resource-type"></a>Тип ресурса Планнерфаворитепланреференце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип ресурса **планнерфаворитепланреференце** репесентс ссылку на [plannerPlan](plannerplan.md) , помеченную пользователем в качестве избранного. Клиенты должны отметить, что записи **планнерфаворитепланреференце** могут ссылаться на **планов** , которые были удалены, что пользователь больше не может получить доступ, или он был обновлен с другим названием.

Мы рекомендуем клиентам уведомлять пользователей о наличии расхождений и постоянном обновлении записей.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|orderHint|String|Указание, используемое для упорядочивания элементов этого типа в списке. Формат определен в статье [Использование указаний order в Планировщике](planner-order-hint-format.md).|
|плантитле|String|Название плана на тот момент, когда пользователь пометил его в качестве избранного.|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReference"
}-->

```json
{
  "orderHint": "String",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


