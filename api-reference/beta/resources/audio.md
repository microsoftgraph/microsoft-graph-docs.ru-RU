---
author: VinodRavichandran
ms.date: 09/10/2017
title: "\"Audio\" (Аудио);"
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f526fc92c766f3ae91831d5026a31e3bd69b4b8b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339110"
---
# <a name="audio-facet"></a>Аспект Audio

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| **bitrate**           | Int32   | Скорость передачи данных в кбит/с.                                           |
| **composers**         | string  | Имя композитора для звукового файла.                          |
| **copyright**         | string  | Сведения об авторском праве для звукового файла.                            |
| **disc**              | Int32   | Номер диска, с которого был взят этот звуковой файл.                    |
| **discCount**         | Int32   | Общее количество дисков для этого альбома.                             |
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

<!--
{
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio",
  "suppressions": []
}
-->
