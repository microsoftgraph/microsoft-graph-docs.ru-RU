---
author: JeremyKelley
ms.date: 09/10/2017
title: Thumbnail
localization_priority: Normal
description: Тип ресурса thumbnail представляет эскиз изображения, видео, документа или любого другого элемента, представленного как растровое изображение.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 76d71cc8cbebc987eea6bbf057945dc41b55f0ee
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239270"
---
# <a name="thumbnail-resource-type"></a>Тип ресурса thumbnail

Пространство имен: microsoft.graph

Тип ресурса **thumbnail** представляет эскиз изображения, видео, документа или любого другого элемента, представленного как растровое изображение.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса **thumbnail** в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "content",
    "height",
    "width",
    "sourceItemId"
  ],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,
  "content": "stream"
}
```

## <a name="properties"></a>Свойства

| Свойство     | Тип   | Описание
| :----------- | :----- | :----------------------------------------------------
| height       | Int32  | Высота эскиза в пикселях.
| sourceItemId | String | Уникальный идентификатор элемента, предоставившего эскиз. Доступен только при запросе эскиза папки.
| url          | String | URL-адрес, используемый для получения содержимого эскиза.
| width        | Int32  | Ширина эскиза в пикселях.
| содержимое      | Поток | Поток содержимого для эскиза.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->

