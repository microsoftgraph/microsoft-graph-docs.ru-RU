---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Фотография
localization_priority: Normal
description: Ресурс photo предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c86190768c10b04bb55f59104368089cf7c77b18
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035501"
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
| **fNumber**             | Двойное         | Значение диафрагмы камеры. Только для чтения.
| **exposureDenominator** | Двойное         | Знаменатель дробного значения выдержки камеры. Только для чтения.
| **exposureNumerator**   | Двойное         | Числитель дробного значения выдержки камеры. Только для чтения.
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
