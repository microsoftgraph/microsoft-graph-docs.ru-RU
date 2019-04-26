---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
ms.openlocfilehash: e3e3305e398651478c88d4c3aa75e753ce26acd5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342047"
---
# <a name="thumbnailset-resource-type"></a>Тип ресурса ThumbnailSet

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet",
  "suppressions": []
}
-->
