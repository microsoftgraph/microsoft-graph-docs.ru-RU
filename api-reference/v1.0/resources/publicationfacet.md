---
title: Тип ресурса publicationFacet
description: Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса driveItemVersion или driveItem.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 91abd61454df2d06131a705dabcb87c9e4ce764f
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806893"
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
