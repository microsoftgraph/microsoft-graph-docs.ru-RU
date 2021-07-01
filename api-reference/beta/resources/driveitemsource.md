---
author: MarcMroz
description: DriveItemSource содержит метаданные об источнике приложения, в которое был создан элемент диска.
title: тип ресурса driveItemSource
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: a403f570ac550b62f9c0e7fa0c3c2fa9758e1772
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236321"
---
# <a name="driveitemsource-resource-type"></a>тип ресурса driveItemSource

Содержит метаданные об источнике элемента диска.

Он доступен в свойстве источника [ресурсов driveItem.][item-resource]

## <a name="properties"></a>Свойства

| Свойство                 | Тип                       | Описание                                                                                      |
| :----------------------- | :------------------------  | :----------------------------------------------------------------------------------------------- |
| **application**          | driveItemSourceApplication | Значение переумерия, которое указывает на источник приложения, в котором был создан файл.              |
| **externalId**           | строка                     | Внешний идентификатор элемента диска из источника.                                      |

### <a name="driveitemsourceapplication-values"></a>значения driveItemSourceApplication

| Значение               | Описание                                       |
|:--------------------|:--------------------------------------------------|
| teams               | Приложение Teams.                         |
| yammer              | Приложение Yammer.                        |
| sharePoint          | Приложение SharePoint.                    |
| oneDrive            | Приложение OneDrive.                      |
| stream              | Приложение — Stream.                        |
| powerPoint          | Приложение PowerPoint                     |
| Office              | Приложение Office                         |
| unknownFutureValue  | Значение маркера для будущей совместимости.            |

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "application",
    "externalId",
  ],
  "@odata.type": "microsoft.graph.driveItemSource"
}-->

```json
{
  "application": "string",
  "externalId" : "string"
}
```

## <a name="see-also"></a>См. также

Дополнительные сведения о гранях на driveItem см. [в сайте driveItem.](driveitem.md)

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The driveItemSource facet provides information about drive item source.",
  "keywords": "driveItemSoruce,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/driveItemSource"
} -->
