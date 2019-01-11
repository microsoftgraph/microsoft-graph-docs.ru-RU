---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: thumbnail
localization_priority: Normal
ms.openlocfilehash: 22602d534c3fd1f308a5e2bb67992bd76086c4fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863226"
---
# <a name="thumbnail-resource-type"></a>Тип ресурса thumbnail

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
