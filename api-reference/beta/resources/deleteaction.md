---
author: daspek
description: Наличие ресурса DeleteAction в ресурсе itemActivity указывает, что в результате выполнения действия элемент был удален.
ms.date: 09/14/2017
title: DeleteAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f5e47f178da27708422e14897a1dd8b19ff328b9
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723502"
---
# <a name="deleteaction-resource-type"></a>Тип ресурса DeleteAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Наличие ресурса **DeleteAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был удален.

[activity]: itemactivity.md

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType&quot;: &quot;File | Folder"
}
```

## <a name="properties"></a>Свойства

| Свойство   | Тип   | Описание                                                    |
| :--------- | :----- | :------------------------------------------------------------- |
| name       | string | Имя элемента, который был удален.                         |
| objectType | string | `File` или `Folder`, в зависимости от типа удаленного элемента. |

## <a name="remarks"></a>Замечания

На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.

<!--
{
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": []
}
-->
