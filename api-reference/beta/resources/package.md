---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Package
localization_priority: Normal
ms.openlocfilehash: 67e82faa3f51eeae71c2dcb22ecb7a973e2070bb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516604"
---
# <a name="package-resource-type"></a>Тип ресурса Package

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **Package** указывает, что элемент DriveItem — это элемент верхнего уровня в "пакете" или коллекции элементов, с которыми следует обращаться как с коллекцией, а не как с отдельными элементами.

Пример пакета — записная книжка OneNote. Несмотря на то что записная книжка состоит из файлов и папок, представляющих ее содержимое, элемент верхнего уровня, который представляет записную книжку, содержит аспект **Package**, с помощью которого можно информировать клиенты о том, что это коллекция данных, с которой необходимо обращаться особым образом.

Элементы DriveItem с аспектом **package** не включают аспект **folder** или **file**, но концептуально похожи на элемент с аспектом **folder**.

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| Имя свойства | Тип   | Описание                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **type**      | string | Строка, обозначающая тип пакета. Несмотря на то что `oneNote` — единственное значение, определенное на данный момент, следует ожидать, что могут быть возвращены пакеты других типов, и иметь возможность обработать их соответствующим образом. |

## <a name="remarks"></a>Заметки 

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).


<!--
{
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/beta/resources/package.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
