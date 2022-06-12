---
title: Тип ресурса publicationFacet
description: Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса driveItemVersion или driveItem.
ms.localizationpriority: medium
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: b2b0f1e329c7dd638d63ffbdc89a9ba891022ce3
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034833"
---
# <a name="publicationfacet-resource-type"></a>Тип ресурса publicationFacet

Пространство имен: microsoft.graph

Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса [driveItemVersion](driveitemversion.md) или [driveItem](driveitem.md).

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a>Свойства

|   Свойство    |  Тип  | Описание |
| :------------ | :----- | :---------- |
| **level**     | String | Состояние публикации для данного документа. Возможные значения: `published` или `checkout`. Только для чтения.  |
| **versionId** | String | Уникальный идентификатор для версии, отображаемый для текущего вызывающего объекта. Только для чтения.  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "suppressions": [
    " Warning: /api-reference/v1.0/resources/publicationfacet.md:
      Found potential enums in resource example that weren't defined in a table:(published,checkout) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Photo"
} -->

