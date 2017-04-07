# <a name="photo-resource-type"></a>Тип ресурса Photo

Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->
```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1024,
  "exposureNumerator": 1024,
  "fNumber": 1024,
  "focalLength": 1024,
  "iso": 1024,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a>Свойства
| Свойство                | Тип                      | Описание                                                     |
|:------------------------|:--------------------------|:----------------------------------------------------------------|
| **takenDateTime**       | DateTimeOffset            | Представляет дату и время съемки. Только для чтения.               |
| **cameraMake**          | Строка                    | Изготовитель камеры. Только для чтения.                                            |
| **cameraModel**         | String                    | Модель камеры. Только для чтения.                                                   |
| **fNumber**             | Double                    | Значение диафрагмы камеры. Только для чтения.                               |
| **exposureDenominator** | Int32                     | Знаменатель дробного значения выдержки камеры. Только для чтения. |
| **exposureNumerator**   | Int32                     | Числитель дробного значения выдержки камеры. Только для чтения.   |
| **focalLength**         | Double                    | Фокусное расстояние камеры. Только для чтения.                               |
| **iso**                 | Int32                     | Значение ISO камеры. Только для чтения.                                  |


## <a name="remarks"></a>Заметки
OneDrive для бизнеса и SharePoint возвращают только свойство **takenDateTime**.

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "photo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
