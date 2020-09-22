---
author: daspek
ms.author: dspektor
title: Тип ресурса moveAction
description: Объект MoveAction предоставляет сведения о действии, которое переместит элемент.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ec1ac8ccaae502f66e205571e17eb5ad3eced8e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020533"
---
# <a name="moveaction-resource-type"></a>Тип ресурса moveAction

Пространство имен: microsoft.graph

Присутствие ресурса **moveAction** в [**itemActivity**][activity] указывает на то, что действие переместило элемент.

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
  "@type": "microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to": "string"
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

