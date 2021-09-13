---
author: JeremyKelley
ms.date: 09/10/2017
title: Изображение
ms.localizationpriority: medium
description: Ресурс Image — это единая структура, объединяющая свойства, связанные с изображением.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a5ccc3baf969199161936ffd635790c56ab75363
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089727"
---
# <a name="image-resource-type"></a>Тип ресурса Image

Пространство имен: microsoft.graph

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

