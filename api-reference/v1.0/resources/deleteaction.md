---
author: daspek
title: тип ресурса deleteAction
description: Объект deleteAction предоставляет сведения об удалении элемента.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e11bf7783bc9c59fe5779c9605acbb4c9e1fb451
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104238"
---
# <a name="deleteaction-resource-type"></a>тип ресурса deleteAction

Пространство имен: microsoft.graph

Наличие ресурса **deleteAction** в [**itemActivity**][activity] указывает на то, что действие удалило элемент.

>**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

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
  "@type&quot;: &quot;microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType&quot;: &quot;File | Folder"
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

