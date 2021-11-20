---
author: JeremyKelley
description: Получение коллекции ресурсов ThumbnailSet для ресурса DriveItem.
ms.date: 09/10/2017
title: Извлечение эскизов для файла или папки
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 3d42771a222d0201fc95d0a7a1913d85118a6588
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2021
ms.locfileid: "61123946"
---
# <a name="list-thumbnails-for-a-driveitem"></a>Список эскизов для ресурса DriveItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [tls-1.2-required](../../includes/tls-1.2-required.md)]

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


## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Для приложений | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$select` для настройки отклика.

Кроме того, этот метод поддерживает ирисовку эскиза с исходным значением EXIF ориентации и без примененного поворота путем придания `originalOrientation=true` параметру запроса.
В настоящее время этот параметр поддерживается только в OneDrive персональный.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ThumbnailSet](../resources/thumbnailset.md) в теле отклика.

## <a name="example"></a>Пример

Ниже представлен пример запроса на получение доступных эскизов элемента в хранилище OneDrive текущего пользователя.


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-item-thumbnails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


Этот запрос возвращает массив доступных объектов **thumbnailSet** для элемента. У любого элемента в объекте drive может быть один или несколько эскизов (либо ни одного эскиза).

**Примечание.** С помощью параметра _select_ строки запроса вы можете указывать размеры эскизов, возвращаемых в объекте **ThumbnailSet**. Например, запрос `/thumbnails?select=medium` получает только эскизы среднего размера.


### <a name="response"></a>Отклик

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

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

## <a name="get-a-single-thumbnail"></a>Получение одного эскиза

Получение метаданных для одного эскиза и размера с помощью прямого запроса.

### <a name="http-request"></a>HTTP-запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-one-thumbnail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a>Параметры пути

| Имя         | Тип   | Описание                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| **item-id**  | string | Уникальный идентификатор элемента.                                           |
| **thumb-id** | число | Индекс эскиза (как правило, 0–4). Если присутствует пользовательский эскиз, для него задается индекс 0. |
| **size**     | string | Размер запрашиваемого эскиза. Это должен быть один из стандартных размеров, указанных ниже, или пользовательский размер. |

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.thumbnail" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "width": 100,
  "height": 100,
  "url": "https://onedrive.com/asd123a/asdjlkasjdkasdjlk.jpg"
}
```

## <a name="retrieve-thumbnail-binary-content"></a>Получение двоичного содержимого эскиза

Вы можете получить содержимое эскиза напрямую, запросив свойство **content** этого эскиза.

### <a name="http-request"></a>HTTP-запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

В ответ служба выполняет перенаправление на URL-адрес эскиза.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

URL-адреса эскизов не кэшируются. Если в результате изменения элемента потребуется создать новый эскиз, изменится его URL-адрес.


## <a name="getting-thumbnails-while-listing-driveitems"></a>Получение эскизов при перечислении ресурсов DriveItem

При получении списка отображаемых ресурсов DriveItem можно использовать параметр строки запроса _$expand_, чтобы также включить эскизы этих ресурсов.
Благодаря этому приложение может получить эскизы и элементы в одном запросе.

### <a name="http-request"></a>HTTP-запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-while-listing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Служба возвращает список ресурсов DriveItem и их эскизов.

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "182331E8-2788-4932-B52A-A6550577043F",
      "name": "my photo.jpg",
      "thumbnails": [
        {
          "small": { "width": 96,
                     "height": 96,
                     "url": "https://sn3302files..."
                   }
        }
      ]
    },
    {
      "id": "2D223953-A56B-4D9B-ADF3-13E7820673A2",
      "name": "presentation.pptx",
      "thumbnails": [
        {
          "small": { "width": 96,
                     "height": 96,
                     "url": "https://sn3302files..."
                   }
        }
      ]
    }
  ]
}
```

## <a name="size-values"></a>Значения размера

В этой таблице определены возможные размеры эскизов. Хотя вы можете указать в запросе произвольный размер эскиза, определенные значения встречаются намного чаще и позволяют быстрее получить результат.

| Имя           | Разрешение  | Пропорции | Описание                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | 96 для большей стороны  | Исходные     | Небольшой эскиз с сильным сжатием, обрезанный до квадрата. |
| `medium`       | 176 для большей стороны | Исходные     | Обрезан до стандартного размера элемента для веб-представления OneDrive.         |
| `large`        | 800 для большей стороны | Исходные     | Эскиз, длина большей стороны которого изменена на 800 пикселей.               |
| `smallSquare`  | 96x96       | Квадратная обрезка  | Небольшой квадратный эскиз                                               |
| `mediumSquare` | 176x176     | Квадратная обрезка  | Небольшой квадратный эскиз                                               |
| `largeSquare`  | 800x800     | Квадратная обрезка  | Большой квадратный эскиз                                               |

## <a name="requesting-custom-thumbnail-sizes"></a>Запрос эскизов настраиваемых размеров

Помимо определенных размеров, приложение может запрашивать эскизы пользовательских размеров, указав ширину и высоту с префиксом `c`.
Например, если вашему приложению нужны эскизы размером 300x400, оно может запросить размер следующим образом:


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request","name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_crop
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-custom-size-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


В ответ вы получите только эскиз выбранного размера:

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "0",
      "c300x400_crop": { "height": 300, "width": 400, "url": "https://sn3302files.onedrive.com/123"},
    }
  ]
}
```

Запросив размер эскиза, вы можете указать следующие параметры:

### <a name="examples-of-custom-identifiers"></a>Примеры пользовательских идентификаторов

| Идентификатор эскиза | Разрешение             | Пропорции | Описание                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| c300x400             | Заключен в прямоугольник размером 300x400 | Исходные     | Создается эскиз, который помещается в прямоугольник размером 300x400 пикселей с сохранением пропорций.                                                                 |
| c300x400_crop        | 300x400                | Обрезанный      | Создается эскиз размером 300x400. Сначала размер изображения меняется так, чтобы оно помещалось в прямоугольник размером 300x400, а затем обрезается все, что выходит за пределы прямоугольника. |

**Примечание.** Размер возвращаемого эскиза в пикселях может не полностью совпадать с запрашиваемым, но его пропорции будут соответствовать запросу.
В некоторых случаях возвращаются эскизы большего размера, если эскиз уже существует и легко масштабируется до запрашиваемого разрешения.

## <a name="remarks"></a>Примечания

**Примечание.** В OneDrive для бизнеса и SharePoint:

С помощью таких вызовов невозможно дополнить коллекцию эскизов:

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

Эскизы не поддерживаются в SharePoint Server 2016.

### <a name="error-responses"></a>Отклики с ошибками

Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "Items/Thumbnails",
  "suppressions": [
  ]
}
-->


