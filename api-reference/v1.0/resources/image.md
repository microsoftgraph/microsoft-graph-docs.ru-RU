---
author: JeremyKelley
title: Тип ресурса image
ms.localizationpriority: medium
description: Ресурс изображения группирует свойства, связанные с образом, в одну структуру.
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 1c457a139504615cde6e21628e82c8875a47b6a9
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900529"
---
# <a name="image-resource-type"></a>Тип ресурса image

Пространство имен: microsoft.graph

Ресурс **изображения** группирует свойства, связанные с образом, в одну структуру.
Если [**driveItem имеет**](driveitem.md) аспект изображения, отличный от **NULL,** элемент представляет точечный рисунок.

>**Примечание:** Если службе не удается определить ширину и высоту изображения, **ресурс изображения может** быть пустым.

## <a name="json-representation"></a>Представление JSON

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

Дополнительные сведения о аспектах в DriveItem см. [в разделе driveItem](driveitem.md).


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->

