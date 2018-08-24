# <a name="imageinfo-resource-type"></a>тип ресурса imageInfo

Сложный тип для представления свойства **атрибуция** в части [visualInfo](../resources/projectrome_visualinfo.md) объекта [активности](../resources/projectrome_activity.md).

## <a name="properties"></a>Свойства

|Имя | Тип | Описание|
|:----|:-----|:-----------|
|IconUrl | Строка | Необязательный параметр; URI-адрес, указывающий на значок, который представляет приложение, используемое для создания действия|
|alternateText | Строка | Необязательный параметр; замещающий текст доступного содержимого для изображения|
|addImageQuery | Логический | Необязательный параметр; предназначенный для указания сервера, может динамически преобразовать изображение для просмотра в ответ на параметризацию. Например, изображение высокой контрастности|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->