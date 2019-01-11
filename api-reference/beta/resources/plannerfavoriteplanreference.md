---
title: Тип ресурса plannerFavoritePlanReference
description: 'Repesents тип **plannerFavoritePlanReference** ресурсов ссылку на plannerPlan, который был помечен как Избранное пользователя. '
localization_priority: Normal
ms.openlocfilehash: b17846eaa1b9a9859d23735d18a191cae4872542
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871325"
---
# <a name="plannerfavoriteplanreference-resource-type"></a>Тип ресурса plannerFavoritePlanReference

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Repesents тип **plannerFavoritePlanReference** ресурсов ссылку на [plannerPlan](plannerplan.md) , который был помечен как Избранное пользователя. Клиенты следует иметь в виду, что записи **plannerFavoritePlanReference** можно ссылаться на **plannerPlans** , будут удалены, пользователь больше не может получить доступ и добавлены иное название.

Рекомендуется уведомлять пользователей есть несоответствия клиентов и обновлять записи.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|orderHint|Строка|Указание, используемое для упорядочивания элементов этого типа в списке. Формат определен в статье [Использование указаний order в Планировщике](planner-order-hint-format.md).|
|planTitle|Строка|Название плана в то время, что пользователь отметил его в список избранного.|


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
<!-- {
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
