---
author: daspek
ms.date: 09/13/2017
title: contentTypeOrder
ms.localizationpriority: medium
description: Ресурс contentTypeOrder указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: be84be025a17677fa6c8546b1a7ccc9f1b3122c0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049594"
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

