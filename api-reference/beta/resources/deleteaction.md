---
author: daspek
description: Наличие ресурса DeleteAction в ресурсе itemActivity указывает, что в результате выполнения действия элемент был удален.
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c5617c61f3221351930ab8d4bf940eaf1efa0629
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973851"
---
# <a name="deleteaction-resource-type"></a>Тип ресурса DeleteAction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Наличие ресурса **DeleteAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был удален.

[activity]: itemactivity.md

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType": "File | Folder"
}
```

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание
|:--------------|:-------|:----------------------------------------------------
| name          | string | Имя элемента, который был удален.
| objectType    | string | `File`или `Folder`, в зависимости от типа удаленного элемента.

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
