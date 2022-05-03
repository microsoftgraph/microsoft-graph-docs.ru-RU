---
author: daspek
description: Наличие ресурса MoveAction в ресурсе itemActivity указывает, что в результате выполнения действия элемент был перемещен.
ms.date: 09/14/2017
title: MoveAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: f3622067f273a587174494d2ce3a68ed56540883
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176552"
---
# <a name="moveaction-resource-type"></a>Тип ресурса MoveAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Наличие ресурса **MoveAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был перемещен.

[activity]: itemactivity.md

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to&quot;: &quot;string"
}
```

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание                                       |
| :------- | :----- | :------------------------------------------------ |
| from     | string | Имя расположения, из которого был перемещен элемент. |
| to       | string | Имя расположения, в которое был перемещен элемент.   |

## <a name="remarks"></a>Замечания

На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.

<!--
{
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction",
  "suppressions": []
}
-->
