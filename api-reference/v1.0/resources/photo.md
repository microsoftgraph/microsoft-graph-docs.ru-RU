---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
ms.openlocfilehash: 4d108e4849595fcb945b676426d3d9c05dfb5ba0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873005"
---
# <a name="photo-resource-type"></a>Тип ресурса Photo

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
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a>Свойства

| Свойство                | Тип           | Описание
|:------------------------|:---------------|:----------------------------------
| **takenDateTime**       | DateTimeOffset | Представляет дату и время съемки. Только для чтения.
| **cameraMake**          | Строка         | Изготовитель камеры. Только для чтения.
| **cameraModel**         | String         | Модель камеры. Только для чтения.
| **fNumber**             | Double         | Значение диафрагмы камеры. Только для чтения.
| **exposureDenominator** | Double         | Знаменатель дробного значения выдержки камеры. Только для чтения.
| **exposureNumerator**   | Double         | Числитель дробного значения выдержки камеры. Только для чтения.
| **focalLength**         | Double         | Фокусное расстояние камеры. Только для чтения.
| **iso**                 | Int32          | Значение ISO камеры. Только для чтения.

## <a name="remarks"></a>Заметки

OneDrive для бизнеса и SharePoint возвращают только свойство **takenDateTime**.

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
