---
author: daspek
ms.author: dspektor
title: Тип ресурса renameAction
description: Объект renameAction предоставляет сведения о действии, которое переименовало элемент.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bce040130d74b7977fc1f988a34edde674f9e0d4
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970803"
---
# <a name="renameaction-resource-type"></a>Тип ресурса renameAction

Присутствие ресурса **renameAction** в [**itemActivity**] [ activity] указывает, что действие переименовало элемент.

>**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

[activity]: itemactivity.md

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание
|:--------------|:-------|:----------------------------------------------------
| oldName       | string | Предыдущее имя элемента.
| Новое       | string | Новое имя элемента.

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.renameAction"
}-->

```json
{
  "oldName": "string",
  "newName": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The renameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/renameAction",
  "suppressions": []
}
-->
