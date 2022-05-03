---
author: daspek
description: Наличие ресурса RenameAction в ресурсе itemActivity указывает, что в результате выполнения действия элемент был переименован.
ms.date: 09/14/2017
title: RenameAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 01ffdffff58b6e7d3592cfa6493d17c3d8649efc
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176866"
---
# <a name="renameaction-resource-type"></a>Тип ресурса RenameAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Наличие ресурса **RenameAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был переименован.

[activity]: itemactivity.md

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.renameAction"
}-->

```json
{
  "oldName": "string",
  "newName&quot;: &quot;string"
}
```

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание                    |
| :------- | :----- | :----------------------------- |
| oldName  | string | Предыдущее имя элемента. |
| Newname  | string | Новое имя элемента.      |

## <a name="remarks"></a>Замечания

На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.

<!--
{
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction",
  "suppressions": []
}
-->
