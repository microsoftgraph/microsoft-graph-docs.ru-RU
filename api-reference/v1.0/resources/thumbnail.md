---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: thumbnail
ms.openlocfilehash: 065c6ae7bbd4f6aca3172afd4399f0a1b5ff3d25
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="thumbnail-resource-type"></a>Тип ресурса thumbnail

Тип ресурса **thumbnail** представляет эскиз изображения, видео, документа или любого другого элемента, представленного как растровое изображение.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса **thumbnail** в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width", "sourceItemId"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,

  /* relationships */
  "content": "stream"
}
```

## <a name="properties"></a>Свойства

| Свойство     | Тип   | Описание                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| height       | Int32  | Высота эскиза в пикселях.                                                                                     |
| sourceItemId | String | Уникальный идентификатор элемента, предоставившего эскиз. Доступен только при запросе эскиза папки. |
| url          | String | URL-адрес, используемый для получения содержимого эскиза.                                                                                |
| width        | Int32  | Ширина эскиза в пикселях.                                                                                      |

## <a name="relationships"></a>Связи

| Имя    | Тип   | Описание                           |
| :------ | :----- | :------------------------------------ |
| content | Stream | Поток содержимого для эскиза. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
