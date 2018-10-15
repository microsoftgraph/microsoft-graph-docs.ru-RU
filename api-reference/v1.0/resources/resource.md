# <a name="onenoteresource-resource-type"></a>Тип ресурса OneNoteResource

Ресурс изображения или другого файла на странице OneNote. 

Вы можете получить двоичные данные ресурса, но получение представления объекта resource или коллекции resource в формате JSON не поддерживается.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "contentUrl": "string (url)"
}
```

Чтобы получить двоичные данные определенного ресурса, отправьте запрос GET в конечную точку `content` ресурса:

```
GET ../onenote/resources/{id}/content
```

При получении HTML-контента страницы с использованием указанного ниже запроса возвращается URI ресурса файла.

```
GET ../onenote/pages/{id}/content
```

На HTML-странице тег `img` включает конечные точки для исходного ресурса изображения в атрибуте `data-fullres-src` и оптимизированного изображения в атрибуте `src`:
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

Тег `object`, который представляет файлы, например PDF-, DOCX- и PNG-файлы, включает конечную точку для ресурса файла в атрибуте `data`:

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a>Свойства

| Свойство             | Тип            | Описание
|:---------------------|:----------------|:---------------------------------
| content              | Stream          | Поток содержимого.
| contentUrl           | Строка (url-адрес)    | URL-адрес загрузки содержимого

## <a name="relationships"></a>Отношения
Нет.


## <a name="methods"></a>Методы
| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получения двоичных данных ресурса](../api/resource_get.md) | Stream |Получение двоичных данных ресурса файла или изображения.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->