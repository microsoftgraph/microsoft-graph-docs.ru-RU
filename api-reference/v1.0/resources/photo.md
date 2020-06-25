---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
description: Ресурс photo предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a62a138cbd48645b6b296abcde72af0cef19e259
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863735"
---
# <a name="photo-resource-type"></a>Тип ресурса Photo

Пространство имен: microsoft.graph

Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->

```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "orientation": 3,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a>Свойства

| Свойство                | Тип           | Описание
|:------------------------|:---------------|:----------------------------------
| **takenDateTime**       | DateTimeOffset | Represents the date and time the photo was taken. Read-only.
| **cameraMake**          | Строка         | Camera manufacturer. Read-only.
| **cameraModel**         | String         | Camera model. Read-only.
| **fNumber**             | Двойное с плавающей точкой         | The F-stop value from the camera. Read-only.
| **exposureDenominator** | Двойное с плавающей точкой         | The denominator for the exposure time fraction from the camera. Read-only.
| **exposureNumerator**   | Двойное с плавающей точкой         | The numerator for the exposure time fraction from the camera. Read-only.
| **focalLength**         | Double         | The focal length from the camera. Read-only.
| **iso**                 | Int32          | The ISO value from the camera. Read-only.
| **orientation**         | Int16          | Значение ориентации камеры. Возможность записи в OneDrive персональный.      |

## <a name="remarks"></a>Заметки

OneDrive для бизнеса и SharePoint возвращают только свойство **takenDateTime**.

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso, orientation",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
