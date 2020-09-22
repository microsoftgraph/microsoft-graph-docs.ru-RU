---
author: JeremyKelley
description: Ресурс Image — это единая структура, объединяющая свойства, связанные с изображением.
ms.date: 09/10/2017
title: Изображение
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: fc7f63c0e7d95c8526d4663b82552541585c9ee2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016641"
---
# <a name="image-resource-type"></a>Тип ресурса Image

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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


<!--
{
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image",
  "suppressions": []
}
-->


