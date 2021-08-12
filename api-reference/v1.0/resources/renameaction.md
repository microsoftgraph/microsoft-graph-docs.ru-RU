---
author: daspek
title: Тип ресурса renameAction
description: Объект renameAction предоставляет сведения о действии, переименовании элемента.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: c1abe3f322f039339514aee0374c0e2e0bd4e3f62aa48534abe37856609cd975
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202135"
---
# <a name="renameaction-resource-type"></a>Тип ресурса renameAction

Пространство имен: microsoft.graph

Наличие ресурса **renameAction** в [**itemActivity**][activity] указывает на то, что действие переименовано в элемент.

>**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

[activity]: itemactivity.md

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание
|:--------------|:-------|:----------------------------------------------------
| oldName       | string | Предыдущее имя элемента.
| newName       | Строка | Новое имя элемента.

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

