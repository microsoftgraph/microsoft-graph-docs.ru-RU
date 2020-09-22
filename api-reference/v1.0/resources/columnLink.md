---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: columnLink
localization_priority: Normal
description: Ресурс columnLink для объекта contentType связывает ресурс columnDefinition сайта с соответствующим типом контента.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4178184b1b9f2fb474783a3d017321c090c5410f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086790"
---
# <a name="columnlink-resource-type"></a>Тип ресурса ColumnLink

Пространство имен: microsoft.graph

Ресурс **columnLink** для объекта [contentType][] связывает ресурс **columnDefinition** сайта с соответствующим типом контента.

[contentType]: contenttype.md

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **columnLink** в формате JSON.
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание
|:--------------|:-------|:----------------------------------------------------
| **id**        | string | Уникальный идентификатор столбца.
| **name**      | string | Имя столбца в этом типе контента.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->

