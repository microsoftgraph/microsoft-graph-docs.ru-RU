---
author: daspek
ms.author: dspektor
title: Тип ресурса deleteAction
description: Объект deleteAction предоставляет сведения об удалении элемента.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ba5004c17f1cc71f66420a81b5eb66603df00eee
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970819"
---
# <a name="deleteaction-resource-type"></a>Тип ресурса deleteAction

Присутствие ресурса **deleteAction** в [**itemActivity**] [ activity] указывает на то, что действие удалило элемент.

>**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

[activity]: itemactivity.md

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание
|:--------------|:-------|:----------------------------------------------------
| name          | string | Имя элемента, который был удален.
| objectType    | string | `File`или `Folder`, в зависимости от типа удаленного элемента.


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

<!--
{
  "type": "#page.annotation",
  "description": "The deleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": []
}
-->
