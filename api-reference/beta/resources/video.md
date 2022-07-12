---
author: JeremyKelley
description: Ресурс Video — это единая структура, объединяющая элементы данных, связанные с видео.
ms.date: 09/10/2017
title: Видео
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 7bd266b8905620bfede51bea0f79c71f6b7f417d
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734671"
---
# <a name="video-resource-type"></a>Тип ресурса video

Пространство имен: microsoft.graph

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
  "height": 1280,
  "width": 720,
  "framerate": 2.75
}
```

## <a name="properties"></a>Свойства

| Свойство                  | Тип   | Описание                                     |
| :------------------------ | :----- | :---------------------------------------------- |
| **audioBitsPerSample**    | Int32  | Количество разрядов звука на выборку.                |
| **audioChannels**         | Int32  | Количество звуковых каналов.                       |
| **audioFormat**           | string | Название формата аудио (AAC, MP3, и т. д.).      |
| **audioSamplesPerSecond** | Int32  | Количество выборок звука в секунду.             |
| **bitrate**               | Int32  | Скорость видео в битах в секунду.       |
| **duration**              | Int64  | Длительность файла в миллисекундах.           |
| **fourCC**                | string | Название формата видео в виде четырехзначного кода. |
| **framerate**             | double | Частота кадров видео.                        |
| **height**                | Int32  | Высота видео в пикселях.                 |
| **width**                 | Int32  | Ширина видео в пикселях.                  |

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
  "suppressions": []
}
-->
