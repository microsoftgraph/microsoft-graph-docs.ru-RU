---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
ms.openlocfilehash: 145134d6a3ad85134ea2d6c4d72e050bc17b31d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830193"
---
# <a name="thumbnailset-resource-type"></a>Тип ресурса ThumbnailSet

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **ThumbnailSet** представляет собой коллекцию ресурсов [thumbnail](thumbnail.md) с ключами. Он представляет набор эскизов, связанных с ресурсом DriveItem.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": ["source", "small", "medium", "large"],
  "openType": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->

```json
{
  "id": "string (identifier)",
  "large": { "@odata.type": "microsoft.graph.thumbnail" },
  "medium": { "@odata.type": "microsoft.graph.thumbnail" },
  "small": { "@odata.type": "microsoft.graph.thumbnail" },
  "source": { "@odata.type": "microsoft.graph.thumbnail" }
}
```

## <a name="properties"></a>Свойства

| Свойство | Тип                      | Описание                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| id       | String                    | Идентификатор в элементе. Только для чтения.                                                |
| large    | [Thumbnail](thumbnail.md) | Эскиз размером 1920x1920.                                                     |
| medium   | [Thumbnail](thumbnail.md) | Эскиз размером 176x176.                                                       |
| small    | [Thumbnail](thumbnail.md) | Обрезанный эскиз размером 48x48.                                                        |
| source   | [Thumbnail](thumbnail.md) | Пользовательский эскиз исходного изображения, используемого для создания других эскизов. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
