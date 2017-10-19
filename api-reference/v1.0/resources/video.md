---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
ms.openlocfilehash: dd6ece46ce54fe791c0e6b5801287e2abad4fe48
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="video-resource-type"></a>Тип ресурса Video

Ресурс **Video** — это единая структура, объединяющая элементы данных, связанные с видео.

Если у ресурса [**DriveItem**](driveitem.md) есть аспект **video**, значение которого не равно null, то этот ресурс представляет видеофайл.
Свойства ресурса **Video** заполняются путем извлечения метаданных из этого файла.

## <a name="json-representation"></a>Представление в формате JSON

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
| **fourCC**                | строка | Название формата видео в виде четырехзначного кода.
| **framerate**             | double | Частота кадров видео.
| **height**                | Int32  | Высота видео в пикселях.
| **width**                 | Int32  | Ширина видео в пикселях.

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>Заметки

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->
