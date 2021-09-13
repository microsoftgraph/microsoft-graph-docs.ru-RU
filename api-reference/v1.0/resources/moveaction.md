---
author: daspek
title: тип ресурса moveAction
description: Объект MoveAction предоставляет сведения о действии, перемещаемом элементом.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 953c932d83060ed650b0e3ad096cf1de40941e1c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067061"
---
# <a name="moveaction-resource-type"></a>тип ресурса moveAction

Пространство имен: microsoft.graph

Наличие ресурса **moveAction** в [**itemActivity**][activity] указывает на то, что действие перемещает элемент.

>**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

[activity]: itemactivity.md

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание
|:--------------|:-------|:----------------------------------------------------
| from          | string | Имя расположения, из которого был перемещен элемент.
| to            | string | Имя расположения, в которое был перемещен элемент.

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

