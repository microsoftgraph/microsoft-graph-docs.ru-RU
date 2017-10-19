---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Image
ms.openlocfilehash: 4488aedaf5c71f6484a0ccf33949fac2569d7af1
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
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
