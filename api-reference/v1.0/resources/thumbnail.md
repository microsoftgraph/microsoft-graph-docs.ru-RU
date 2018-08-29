---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: thumbnail
ms.openlocfilehash: ff111f44101bb03b3d8475e2567d6e1b2b4a753d
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264975"
---
# <a name="thumbnail-resource-type"></a>Тип ресурса thumbnail

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
| sourceItemId | строка | Уникальный идентификатор элемента, предоставившего эскиз. Доступен только при запросе эскиза папки.
| url          | строка | URL-адрес, используемый для получения содержимого эскиза.
| width        | Int32  | Ширина эскиза в пикселях.
| content      | Stream | Поток содержимого для эскиза.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
