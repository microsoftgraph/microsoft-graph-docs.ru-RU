---
author: JeremyKelley
title: Скачивание файла
ms.localizationpriority: high
ms.prod: sharepoint
description: Скачивание содержимого основного потока (файла) элемента driveItem. Можно скачать только те ресурсы driveItem, у которых есть свойство file.
doc_type: apiPageType
ms.openlocfilehash: 5e5e3a2b9d174957b80c0a74e96d3a658279e44d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336335"
---
# <a name="download-the-contents-of-a-driveitem"></a>Скачивание содержимого элемента DriveItem

Пространство имен: microsoft.graph

[!INCLUDE [tls-1.2-required](../../includes/tls-1.2-required.md)]

Скачивание содержимого основного потока (файла) элемента [driveItem](../resources/driveitem.md). Вы можете скачать только те элементы **driveItem**, у которых есть свойство **file**.

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
GET /drives/{drive-id}/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /shares/{shareIdOrEncodedSharingUrl}/driveItem/content
GET /sites/{siteId}/drive/items/{item-id}/content
GET /users/{userId}/drive/items/{item-id}/content
```

## <a name="optional-request-headers"></a>Необязательные заголовки запросов

| Имя          | Значение  | Описание                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | String | Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`. |

## <a name="example"></a>Пример

В примере ниже показано, как скачать весь файл.

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "download-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/content
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/download-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/download-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/download-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/download-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Возвращает отклик `302 Found`, перенаправляя к URL-адресу загрузки файла, прошедшему предварительную проверку подлинности. Это такой же URL-адрес, доступный с помощью свойства `@microsoft.graph.downloadUrl` в ресурсе DriveItem.

Чтобы скачать содержимое файла, приложению необходимо следовать заголовку `Location` в отклике. Многие библиотеки клиентов HTTP будут автоматически следовать перенаправлению 302 и немедленно начинать скачивание файла.

URL-адреса загрузки, прошедшие предварительную проверку подлинности, действительны только на протяжении короткого периода времени (несколько минут) и не требуют заголовка `Authorization` для загрузки.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="downloading-files-in-javascript-apps"></a>Скачивание файлов в приложениях на JavaScript
Для скачивания файлов в приложении на JavaScript невозможно использовать API `/content`, так как при этом возвращается код перенаправления `302`. Перенаправление с помощью кода `302` запрещено, если требуется _предварительная проверка_ [общего доступа к ресурсам независимо от источника (CORS)](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS), например когда указан заголовок **Authorization**.

Вместо этого приложение должно выбрать свойство `@microsoft.graph.downloadUrl`, возвращающее тот же URL-адрес, на который перенаправляет ссылка `/content`.
Затем этот URL-адрес можно запросить напрямую с помощью XMLHttpRequest.
Так как эти URL-адреса прошли предварительную проверку подлинности, их можно получить без запроса предварительной проверки CORS.

### <a name="example"></a>Пример

Чтобы получить URL-адрес для скачивания файла, сначала отправьте запрос, включающий свойство `@microsoft.graph.downloadUrl`:

```http
GET /drive/items/{item-ID}?select=id,@microsoft.graph.downloadUrl
```

При этом возвращаются идентификатор и URL-адрес для скачивания файла:

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "12319191!11919",
  "@microsoft.graph.downloadUrl": "https://..."
}
```

Затем вы можете отправить запрос XMLHttpRequest на URL-адрес, указанный в свойстве `@microsoft.graph.downloadUrl`, чтобы получить файл.

## <a name="partial-range-downloads"></a>Загрузка части заданного диапазона байтов

Чтобы загрузить из файла часть заданного диапазона байтов, приложение может использовать заголовок `Range`, как указано в документе [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Обратите внимание, что заголовок `Range` необходимо добавлять в фактический URL-адрес `@microsoft.graph.downloadUrl`, а не в запрос для `/content`.

<!-- { "blockType": "request", "opaqueUrl": true, "name": "download-item-partial", "scopes": "files.read" } -->

```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

Это позволит вернуть отклик `HTTP 206 Partial Content` с запрашиваемым диапазоном байтов из файла. Если не удается создать диапазон, можно проигнорировать заголовок диапазона, после чего отклик `HTTP 200` возвращается с полным содержимым файла.

<!-- { "blockType": "response", "name": "download-item-partial", "@odata.type": "stream" } -->

```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048
Content-Type: application/octet-stream

<first 1024 bytes of file>
```

### <a name="error-responses"></a>Ответы с ошибками

Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Download the contents of a DriveItem.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Items/Download",
  "suppressions": [
  ]
} -->

