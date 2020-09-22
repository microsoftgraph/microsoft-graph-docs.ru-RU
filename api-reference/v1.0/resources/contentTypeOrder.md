---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: contentTypeOrder
localization_priority: Normal
description: Ресурс contentTypeOrder указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2015b0def71ece538fddafde407e8bf044375b4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056942"
---
# <a name="contenttypeorder-resource-type"></a>Тип ресурса contentTypeOrder

Пространство имен: microsoft.graph

Ресурс **contentTypeOrder** указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **contentTypeOrder** в формате JSON.
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a>Свойства

| Имя свойства | Тип    | Описание
|:--------------|:--------|:----------------------------------------------------
| **default**   | boolean | Указывает, используется ли этот тип контента по умолчанию.
| **position**  | Int32   | Указывает позицию, в которой тип контента отображается в пользовательском интерфейсе выбора.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->

