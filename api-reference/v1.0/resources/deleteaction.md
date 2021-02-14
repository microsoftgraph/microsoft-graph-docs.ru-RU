---
author: daspek
title: Тип ресурса deleteAction
description: Объект deleteAction предоставляет сведения об удалении элемента.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e78b4369606b0e0e3880fc3bfd13fdec263fcb58
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239634"
---
# <a name="deleteaction-resource-type"></a>Тип ресурса deleteAction

Пространство имен: microsoft.graph

Наличие ресурса **deleteAction** в [**itemActivity**][activity] указывает, что действие удалило элемент.

>**Примечание.** Записи о действиях с элементами в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

[activity]: itemactivity.md

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание
|:--------------|:-------|:----------------------------------------------------
| name          | string | Имя элемента, который был удален.
| objectType    | string | `File` или `Folder` , в зависимости от типа удаленного элемента.


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

