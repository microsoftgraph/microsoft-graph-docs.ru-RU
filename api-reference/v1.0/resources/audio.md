---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Звук
ms.openlocfilehash: e68b70565f0eccd7847fba2b8085661071a75ae7
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266235"
---
# <a name="audio-facet"></a>Аспект Audio

Ресурс **Звук** группирует свойства элемента, связанные со звуком, в единую структуру.

Если у элемента [**DriveItem**](driveitem.md) есть ненулевой аспект **audio**, то этот элемент представляет звуковой файл. Свойства ресурса **Audio** заполняются путем извлечения метаданных из такого файла. 

## <a name="json-representation"></a>Представление JSON

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
| **альбом**             | строка  | Название альбома для этого звукового файла.                          |
| **albumArtist**       | строка  | Название исполнителя альбома для этого звукового файла.                    |
| **исполнитель**            | строка  | Исполнитель для звукового файла.                            |
| **Скорость**           | Int64   | Скорость передачи данных в кбит/с.                                           |
| **композиторы**         | строка  | Имя композитора для звукового файла.                          |
| **авторское право**         | строка  | Сведения об авторском праве для звукового файла.                            |
| **диск**              | Int16   | Номер диска, с которого был взят этот звуковой файл.                    |
| **discCount**         | Int16   | Общее количество дисков в этом альбоме.                             |
| **длительность**          | Int64   | Длительность воспроизведения звукового файла в миллисекундах.                |
| **жанр**             | строка  | Жанр этого звукового файла.                                        |
| **hasDrm**            | логический | Указывает, защищен ли файл с помощью технологии управления цифровыми правами.   |
| **isVariableBitrate** | логический | Указывает, закодирован ли файл с использованием переменной скорости передачи данных.            |
| **название**             | строка  | Название звукового файла.                                         |
| **дорожка**             | Int32   | Номер дорожки на исходном диске для этого звукового файла.    |
| **trackCount**        | Int32   | Общее количество дорожек на исходном диске для этого звукового файла. |
| **год**              | Int32   | Год записи звукового файла.                                |

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
