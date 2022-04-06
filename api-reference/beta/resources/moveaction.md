---
author: daspek
description: Наличие ресурса MoveAction в ресурсе itemActivity указывает, что в результате выполнения действия элемент был перемещен.
ms.date: 09/14/2017
title: MoveAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d5da0b6502752f25ad59b9d19a8a4a366d473ec8
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722659"
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
