---
author: ananmishr
ms.date: 09/10/2017
title: "\"Audio\" (Аудио);"
localization_priority: Normal
ms.prod: microsoft-teams
description: Ресурс Audio группирует свойства элемента, связанные со звуком, в единую структуру.
doc_type: resourcePageType
ms.openlocfilehash: 1351ae9dcd363d156997fd5cc75e7e3387a0fb38
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913487"
---
# <a name="audio-facet"></a>Аспект Audio

Ресурс **Audio** группирует свойства элемента, связанные со звуком, в единую структуру.

Если у элемента [**DriveItem**](driveitem.md) есть ненулевой аспект **audio**, то этот элемент представляет звуковой файл. Свойства ресурса **Audio** заполняются путем извлечения метаданных из такого файла. 

## <a name="json-representation"></a>Представление в формате JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.audio" } -->
```json
{
  "album": "string",
  "albumArtist": "string",
  "artist": "string",
  "bitrate": 128,
  "composers": "string",
  "copyright": "string",
  "disc": 0,
  "discCount": 0,
  "duration": 567,
  "genre": "string",
  "hasDrm": false,
  "isVariableBitrate": false,
  "title": "string",
  "track": 1,
  "trackCount": 16,
  "year": 2014
}
```

## <a name="properties"></a>Свойства

| Имя свойства         | Тип    | Описание                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| **album**             | string  | Название альбома для этого звукового файла.                          |
| **albumArtist**       | string  | Название исполнителя альбома для этого звукового файла.                    |
| **artist**            | string  | Исполнитель для звукового файла.                            |
| **bitrate**           | Int64   | Скорость передачи данных в кбит/с.                                           |
| **composers**         | string  | Имя композитора для звукового файла.                          |
| **copyright**         | string  | Сведения об авторском праве для звукового файла.                            |
| **disc**              | Int16   | Номер диска, с которого был взят этот звуковой файл.                    |
| **discCount**         | Int16   | Общее количество дисков для этого альбома.                             |
| **duration**          | Int64   | Длительность воспроизведения звукового файла в миллисекундах.                |
| **genre**             | string  | Жанр этого звукового файла.                                        |
| **hasDrm**            | boolean | Указывает, защищен ли файл с помощью технологии управления цифровыми правами.   |
| **isVariableBitrate** | boolean | Указывает, закодирован ли файл с использованием переменной скорости передачи данных.            |
| **title**             | строка  | Название звукового файла.                                         |
| **track**             | Int32   | Номер дорожки на исходном диске для этого звукового файла.    |
| **trackCount**        | Int32   | Общее количество дорожек на исходном диске для этого звукового файла. |
| **year**              | Int32   | Год записи звукового файла.                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>Примечания

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
