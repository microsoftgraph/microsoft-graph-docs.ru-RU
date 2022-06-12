---
author: JeremyKelley
ms.date: 09/10/2017
title: photo;
ms.localizationpriority: medium
description: Ресурс photo предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе driveItem.
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 80bcc486e6e577ebde22925f16e79c83e32f8cae
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034469"
---
# <a name="photo-resource-type"></a>Тип ресурса photo

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
| **takenDateTime**       | DateTimeOffset | Представляет дату и время съемки. Только для чтения.
| **cameraMake**          | Строка         | Изготовитель камеры. Только для чтения.
| **cameraModel**         | String         | Модель камеры. Только для чтения.
| **fNumber**             | Double         | Значение диафрагмы камеры. Только для чтения.
| **exposureDenominator** | Double         | Знаменатель дробного значения выдержки камеры. Только для чтения.
| **exposureNumerator**   | Double         | Числитель дробного значения выдержки камеры. Только для чтения.
| **focalLength**         | Double         | Фокусное расстояние камеры. Только для чтения.
| **iso**                 | Int32          | Значение ISO камеры. Только для чтения.
| **orientation**         | Int16          | Значение ориентации камеры. Доступно для записи в OneDrive Персональный.      |

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

