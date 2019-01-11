---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Image
localization_priority: Normal
ms.openlocfilehash: 4526b8d475b36521ee08829b50931438999ca249
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830417"
---
# <a name="image-resource-type"></a>Тип ресурса Image

Ресурс **Image** — это единая структура, объединяющая свойства, связанные с изображением. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **image**, то этот ресурс представляет точечный рисунок.

**Примечание.** Если службе не удается определить ширину и высоту изображения, ресурс **Image** может быть пустым.

## <a name="json-representation"></a>Описание в формате JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a>Свойства

| Свойство   | Тип  | Описание                                |
|:-----------|:------|:-------------------------------------------|
| **height** | Int32 | Необязательный. Высота изображения в пикселях. Только для чтения. |
| **width**  | Int32 | Необязательный. Ширина изображения в пикселях. Только для чтения.  |

## <a name="remarks"></a>Заметки

В OneDrive для бизнеса этот ресурс возвращается для элементов, которые должны быть изображениями в соответствии с расширением файла.

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
