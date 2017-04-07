# <a name="video-resource-type"></a>Тип ресурса Video

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
  "bitrate": 1024,
  "duration": 1024,
  "height": 1024,
  "width": 1024
}
```

## <a name="properties"></a>Свойства

| Свойство | Тип  | Описание                               |
|:---------|:------|:------------------------------------------|
| bitrate  | Int32 | Скорость видео в битах в секунду. |
| duration | Int64 | Продолжительность файла в миллисекундах.     |
| height   | Int32 | Высота видео в пикселях.           |
| width    | Int32 | Ширина видео в пикселях.            |

## <a name="remarks"></a>Заметки 

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "video resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
