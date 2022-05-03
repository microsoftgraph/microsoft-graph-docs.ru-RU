---
title: Тип ресурса photo
description: Ресурс photo предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе driveItem.
ms.date: 09/10/2017
ms.localizationpriority: medium
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: bc253cd90a75438f627cf00c55551cfb8bc12d01
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176352"
---
# <a name="photo-resource-type"></a>Тип ресурса photo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).

> [!NOTE]
> В настоящее **время только takenDateTime** доступен в OneDrive для бизнеса и SharePoint.

## <a name="properties"></a>Свойства

| Свойство          | Тип          | Описание                                                                |
|:------------------|:--------------|:---------------------------------------------------------------------------|
|cameraMake         |Строка         | Изготовитель камеры. Только для чтения.                                            |
|cameraModel        |String         | Модель камеры. Только для чтения.                                                   |
|exposureDenominator|Double         | Знаменатель дробного значения выдержки камеры. Только для чтения. |
|exposureNumerator  |Double         | Числитель дробного значения выдержки камеры. Только для чтения.   |
|fNumber            |Double         | Значение диафрагмы камеры. Только для чтения.                               |
|focalLength        |Double         | Фокусное расстояние камеры. Только для чтения.                               |
|iso                |Int32          | Значение ISO камеры. Только для чтения.                                  |
|orientation        |Int16          | Значение ориентации камеры. Доступно для записи в OneDrive Персональный.      |
|takenDateTime      |DateTimeOffset | Дата и время создания фотографии в формате UTC. Только для чтения.              |

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


