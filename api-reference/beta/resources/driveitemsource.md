---
author: MarcMroz
description: DriveItemSource содержит метаданные об источнике приложения, в которое был создан элемент диска.
title: тип ресурса driveItemSource
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: eada8fa22672a80d712ef78be5cc3d44ac354216
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59047459"
---
# <a name="driveitemsource-resource-type"></a>тип ресурса driveItemSource

Содержит метаданные об источнике элемента диска.

Он доступен в свойстве источника [ресурсов driveItem.][item-resource]

## <a name="properties"></a>Свойства

| Свойство                 | Тип                       | Описание                                                                                      |
| :----------------------- | :------------------------  | :----------------------------------------------------------------------------------------------- |
| **application**          | driveItemSourceApplication | Значение переумерия, которое указывает на источник приложения, в котором был создан файл.              |
| **externalId**           | String                     | Внешний идентификатор элемента диска из источника.                                      |

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
