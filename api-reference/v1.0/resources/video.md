---
author: JeremyKelley
title: Тип видео ресурса
ms.localizationpriority: medium
description: Видеоматериалы группирует элементы данных, связанные с видео, в одну структуру.
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 81a2ccd6250261c87b5af84cc0bef0ace4342702
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65897827"
---
# <a name="video-resource-type"></a>Тип видео ресурса

Пространство имен: microsoft.graph

**Видеоматериалы** группирует элементы данных, связанные с видео, в одну структуру.

Если [**driveItem**](driveitem.md) имеет аспект видео, отличный от **NULL,** элемент представляет видеофайл.
Свойства видео ресурса **заполняются** путем извлечения метаданных из файла.

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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
| **Кадров**             | double | Частота кадров видео.
| **height**                | Int32  | Высота видео в пикселях.
| **width**                 | Int32  | Ширина видео в пикселях.

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>Заметки

Дополнительные сведения о аспектах на driveItem см. в [разделе driveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->

