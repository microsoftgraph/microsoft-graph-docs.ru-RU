# <a name="audio-resource-type"></a>Тип ресурса Audio

Ресурс **Audio** группирует свойства элемента, связанные со звуком, в единую структуру.

Если у элемента [**DriveItem**](driveitem.md) есть ненулевой аспект **audio**, то этот элемент представляет звуковой файл. Свойства ресурса **Audio** заполняются путем извлечения метаданных из такого файла. 

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.audio"
}-->
```json
{
  "album": "string",
  "albumArtist": "string",
  "artist": "string",
  "bitrate": 1024,
  "composers": "string",
  "copyright": "string",
  "disc": 1024,
  "discCount": 1024,
  "duration": 1024,
  "genre": "string",
  "hasDrm": true,
  "isVariableBitrate": true,
  "title": "string",
  "track": 1024,
  "trackCount": 1024,
  "year": 1024
}
```

## <a name="properties"></a>Свойства

| Свойство          | Тип    | Описание                                                          |
|:------------------|:--------|:---------------------------------------------------------------------|
| album             | string  | Название альбома для этого звукового файла.                          |
| albumArtist       | string  | Название исполнителя альбома для этого звукового файла.                    |
| artist            | string  | Исполнитель для звукового файла.                            |
| bitrate           | string  | Битрейт в Кбит/с.                                           |
| composers         | string  | Имя композитора для звукового файла.                          |
| copyright         | string  | Сведения об авторском праве для звукового файла.                            |
| disc              | number  | Номер диска, с которого был взят этот звуковой файл.                    |
| discCount         | number  | Количество дисков для этого альбома.                             |
| duration          | number  | Длительность воспроизведения звукового файла в миллисекундах.                |
| genre             | string  | Жанр этого звукового файла.                                        |
| hasDrm            | boolean | Указывает, защищен ли файл с помощью управления цифровыми правами.   |
| isVariableBitrate | boolean | Указывает, закодирован ли файл с использованием переменного битрейта.            |
| title             | string  | Название звукового файла.                                         |
| track             | number  | Номер композиции на первоначальном диске для этого звукового файла.    |
| trackCount        | number  | Общее количество композиций на первоначальном диске для этого звукового файла. |
| year              | number  | Год записи звукового файла.                                |

## <a name="remarks"></a>Примечания 

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audio resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->