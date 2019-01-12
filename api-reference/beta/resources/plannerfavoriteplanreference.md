---
title: Тип ресурса plannerFavoritePlanReference
description: 'Repesents тип **plannerFavoritePlanReference** ресурсов ссылку на plannerPlan, который был помечен как Избранное пользователя. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 48dabeb83522c4151f9da2db9192c7ad546a9bc8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938274"
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
