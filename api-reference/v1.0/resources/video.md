---
author: JeremyKelley
ms.date: 09/10/2017
title: Видео
ms.localizationpriority: medium
description: Ресурс Video — это единая структура, объединяющая элементы данных, связанные с видео.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d46949bf48455fbb74a99891a80984bdedb460fb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134271"
---
# <a name="video-resource-type"></a>Тип ресурса video

Пространство имен: microsoft.graph

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
| **audioFormat**           | string | Название формата аудио (AAC, MP3, и т. д.).
| **audioSamplesPerSecond** | Int32  | Количество выборок звука в секунду.
| **bitrate**               | Int32  | Скорость видео в битах в секунду.
| **duration**              | Int64  | Длительность файла в миллисекундах.
| **fourCC**                | string | Название формата видео в виде четырехзначного кода.
| **frameRate**             | double | Частота кадров видео.
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

