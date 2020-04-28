---
title: Тип ресурса Photo
description: Ресурс photo предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе driveItem.
ms.date: 09/10/2017
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bdb587e7440fd98c48f71a2611e2a34e039367dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521885"
---
# <a name="photo-resource-type"></a>Тип ресурса Photo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).

> [!NOTE]
> В настоящее время в OneDrive для бизнеса и SharePoint доступен только **takenDateTime** .

## <a name="properties"></a>Свойства

| Свойство          | Тип          | Описание                                                                |
|:------------------|:--------------|:---------------------------------------------------------------------------|
|cameraMake         |Строка         | Изготовитель камеры. Только для чтения.                                            |
|cameraModel        |String         | Модель камеры. Только для чтения.                                                   |
|exposureDenominator|Двойное с плавающей точкой         | Знаменатель дробного значения выдержки камеры. Только для чтения. |
|exposureNumerator  |Двойное с плавающей точкой         | Числитель дробного значения выдержки камеры. Только для чтения.   |
|fNumber            |Двойное с плавающей точкой         | Значение диафрагмы камеры. Только для чтения.                               |
|focalLength        |Double         | Фокусное расстояние камеры. Только для чтения.                               |
|iso                |Int32          | Значение ISO камеры. Только для чтения.                                  |
|orientation        |Int16          | Значение ориентации камеры. Возможность записи в OneDrive персональный.      |
|takenDateTime      |DateTimeOffset | Дата и время, когда фотография заняла время в формате UTC. Только для чтения.              |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.photo",
  "baseType": null
}-->

```json
{
  "cameraMake": "String",
  "cameraModel": "String",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "orientation": 3,
  "takenDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The photo resource provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso, orientation",
  "section": "documentation",
  "tocPath": ""
}-->
