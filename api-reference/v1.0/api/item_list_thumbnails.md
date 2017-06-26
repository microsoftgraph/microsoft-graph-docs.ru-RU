# <a name="list-thumbnails-for-a-driveitem"></a>Список эскизов для ресурса DriveItem

Получение коллекции ресурсов [ThumbnailSet](../resources/thumbnailset.md) для ресурса [DriveItem](../resources/driveitem.md).

Ресурс DriveItem представляют ресурсы [ThumbnailSet](../resources/thumbnailset.md), количество которых может быть нуль и более. Каждый ресурс **thumbnailSet** может включать один или несколько объектов [**thumbnail**](../resources/thumbnail.md) — изображений, представляющих элемент. К примеру, ресурс **thumbnailSet** может включать такие распространенные объекты **thumbnail**, как `small`, `medium` и `large`.

Работать с эскизами в OneDrive можно множеством способов. Ниже представлены наиболее распространенные из них.

* Перечисление доступных эскизов элемента
* Получение одного эскиза элемента
* Получение содержимого эскиза
* Получение эскизов нескольких элементов в одном запросе
* Получение эскизов настраиваемых размеров
* Отправка пользовательского эскиза элемента
* Определение того, существует ли отправленный пользовательский эскиз


## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из указанных **областей**:

* Files.Read
* Files.ReadWrite.
* Files.Read.All
* Files.ReadWrite.All
* Sites.Read.All
* Sites.ReadWrite.All


## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ThumbnailSet](../resources/thumbnailset.md) в теле отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "get_thumbnails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails
```


##### <a name="response"></a>Отклик
Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailSet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0",
      "small": { "height": 64, "width": 96, "url": "https://sn3302files..."},
      "medium": { "height": 117, "width": 176, "url": "https://sn3302files..."},
      "large": { "height": 533, "width": 800, "url": "https://sn3302files..."}
    }
  ]
}
```

## <a name="retrieve-a-single-thumbnail"></a>Получение одного эскиза

Получение метаданных для одного эскиза и размера с помощью прямого запроса.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "request", "name": "get-one-thumbnail" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

## <a name="path-parameters"></a>Параметры пути

| Имя         | Тип   | Описание                                                                         |
|:-------------|:-------|:------------------------------------------------------------------------------------|
| **item-id**  | string | Уникальный идентификатор элемента.                                      |
| **thumb-id** | number | Индекс эскиза (как правило, 0–4).                                            |
| **size**     | string | Размер запрашиваемого эскиза. Это должен быть один из указанных стандартных размеров. |


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.thumbnail" } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "width": 100,
  "height": 100,
  "url": "http://onedrive.com/asd123a/asdjlkasjdkasdjlk.jpg"
}
```

## <a name="retrieve-thumbnail-content"></a>Получение содержимого эскиза

Вы можете получить содержимое эскиза напрямую, запросив свойство **content** этого эскиза.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "request", "name":"get-thumbnail-content" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

## <a name="response"></a>Отклик

В ответ служба перенаправляет на URL-адрес эскиза.

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

Для URL-адресов содержимого эскизов выполняется предварительная проверка подлинности, поэтому они не требуют скачивания заголовка авторизации. Эти URL-адреса действительны в течение нескольких часов, поэтому их не следует кэшировать в приложениях.


## <a name="size-values"></a>Значения размера

В этой таблице определены возможные размеры эскизов. Хотя вы можете указать в запросе произвольный размер эскиза, определенные значения встречаются намного чаще и позволяют быстрее получить результат.

| Имя           | Разрешение  | Пропорции | Описание                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | 96 для большей стороны  | Исходные     | Небольшой эскиз с сильным сжатием, обрезанный до квадрата. |
| `medium`       | 176 для большей стороны | Исходные     | Обрезан до стандартного размера элемента для веб-представления OneDrive.         |
| `large`        | 800 для большей стороны | Исходные     | Эскиз, длина большей стороны которого изменена на 800 пикселей.               |

## <a name="remarks"></a>Заметки

**Примечание.** В OneDrive для бизнеса и SharePoint:

* С помощью таких вызовов невозможно дополнить коллекцию эскизов: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`.


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List thumbnails"
} -->
