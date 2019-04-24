---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Видео
localization_priority: Normal
ms.openlocfilehash: 1e780c8392316be1f7fcc59f3818085dc462da29
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454025"
---
# <a name="video-resource-type"></a>Тип ресурса video

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **Video** — это единая структура, объединяющая элементы данных, связанные с видео.

Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **video**, то этот ресурс представляет видеофайл. Свойства ресурса **Video** заполняются путем извлечения метаданных из такого файла.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.video"
}-->

```json
{
  "audioBitsPerSample": 16,
  "audioChannels": 1,
  "audioFormat": "AAC",
  "audioSamplesPerSecond": 44100,
  "bitrate": 39101896,
  "duration": 8053,
  "fourCC": "H264",
  "frameRate": 239.877,
  "height": 1280,
  "width": 720
}
```

## <a name="properties"></a>Свойства

| Имя свойства             | Тип   | Описание
|:--------------------------|:-------|:----------------------------------------
| **audioBitsPerSample**    | Int32  | Количество разрядов звука на выборку.
| **audioChannels**         | Int32  | Количество звуковых каналов.
| **audioFormat**           | строка | Название формата аудио (AAC, MP3, и т. д.).
| **audioSamplesPerSecond** | Int32  | Количество выборок звука в секунду.
| **bitrate**               | Int32  | Скорость видео в битах в секунду.
| **duration**              | Int64  | Длительность файла в миллисекундах.
| **fourCC**                | string | Название формата видео в виде четырехзначного кода.
| **framerate**             | double | Частота кадров видео.
| **height**                | Int32  | Высота видео в пикселях.
| **width**                 | Int32  | Ширина видео в пикселях.

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>Заметки

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/video.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
