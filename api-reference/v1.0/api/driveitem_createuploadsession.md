---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Возобновляемая отправка файлов
ms.openlocfilehash: 14b9047f84b5390aea2f5285660e6c04a6bc3149
ms.sourcegitcommit: ebac77d2ca32438e552831de0258fe5e86fa225a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2018
ms.locfileid: "26564760"
---
# <a name="upload-large-files-with-an-upload-session"></a>Отправка больших файлов с помощью сеанса отправки

Создайте сеанс отправки, чтобы приложение могло отправлять файлы, размер которых не превышает максимальный. С помощью сеанса отправки приложение может отправлять диапазоны файла при последовательных запросах API, что позволяет возобновить передачу, если во время отправки соединение будет разорвано.

Процесс отправки файла с помощью сеанса отправки состоит из двух этапов:

1. [Создание сеанса отправки](#create-an-upload-session).
2. [Отправка байтов в сеанс отправки](#upload-bytes-to-the-upload-session).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite, Files.ReadWrite.All    |
|Для приложений | Sites.ReadWrite.All |

## <a name="create-an-upload-session"></a>Создание сеанса отправки

Чтобы начать отправку большого файла, приложение должно сначала запросить новый сеанс отправки. При этом создается временное место хранения, где сохраняются байты файла, пока он не будет отправлен полностью. После отправки последнего байта файла сеанс отправки завершается, а готовый файл отображается в целевой папке.

### <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createUploadSession
POST /groups/{groupId}/drive/items/{itemId}/createUploadSession
POST /me/drive/items/{itemId}/createUploadSession
POST /sites/{siteId}/drive/items/{itemId}/createUploadSession
POST /users/{userId}/drive/items/{itemId}/createUploadSession
```

### <a name="request-body"></a>Текст запроса

Тело запроса не требуется.
Тем не менее, можно указать `item` свойство в тексте запроса, предоставляя дополнительные данные о выгружаемого файла.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } -->
```json
{
  "@microsoft.graph.conflictBehavior": "rename | fail | replace",
  "description": "description",
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "name": "filename.txt"
}
```

Например, вы можете задать необходимые действия для случая, когда имя файла уже используется, указав в теле запроса свойство поведения при конфликтах.

<!-- { "blockType": "ignored" } -->
```json
{
  "item": {
    "@microsoft.graph.conflictBehavior": "rename"
  }
}
```

### <a name="optional-request-headers"></a>Необязательные заголовки запросов

| Имя       | Значение | Описание                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| *if-match* | etag  | Если указан заголовок запроса, а предоставленное значение eTag (или cTag) не совпадает с текущим значением eTag элемента, то возвращается ошибка `412 Precondition Failed`. |

## <a name="properties"></a>Свойства

| Свойство             | Тип               | Описание
|:---------------------|:-------------------|:---------------------------------
| описание          | String             | Предоставляет видимое пользователю описание элемента. Чтение и запись. Только в личном хранилище OneDrive
| fileSystemInfo       | [fileSystemInfo][] | Сведения о файловой системе на клиенте. Чтение и запись.
| name                 | String             | Имя элемента (имя и расширение файла). Чтение и запись.

### <a name="request"></a>Запрос

В отклике на этот запрос будут представлены подробные сведения о новом экземпляре [uploadSession](../resources/uploadsession.md) (в том числе URL-адрес для отправки фрагментов файла). 

<!-- { "blockType": "request", "name": "upload-fragment-create-session", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/root:/{item-path}:/createUploadSession
Content-Type: application/json

{
  "item": {
    "@odata.type": "microsoft.graph.driveItemUploadableProperties",
    "@microsoft.graph.conflictBehavior": "rename",
    "name": "largefile.dat"
  }
}
```

### <a name="response"></a>Ответ

В случае успешного выполнения запроса ответ будет содержать сведения о том, куда отправлять остальные запросы (в виде ресурса [UploadSession](../resources/uploadSession.md)).

Этот ресурс предоставляет сведения о том, куда следует отправлять диапазон байтов файла и когда истекает срок действия сеанса отправки.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession",
       "optionalProperties": [ "nextExpectedRanges" ]  } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z"
}
```

## <a name="upload-bytes-to-the-upload-session"></a>Отправка байтов в сеанс отправки

Чтобы отправить файл или его часть, приложение выполняет запрос PUT на адрес **uploadUrl**, указанный в отклике для **createUploadSession**.
Вы можете отправить файл целиком или разделить его на несколько диапазонов байтов. При этом каждый запрос должен содержать фрагмент размером не более 60 МБ.

Фрагменты файл должен загружаться последовательно в порядке.
В противном случае возникнет ошибка.

**Примечание.** Если приложение делит файл на несколько диапазонов байтов, размер каждого из них **ДОЛЖЕН** быть кратным 320 КБ (327 680 байтов). Если размер фрагментов не делится на 320 КБ без остатка, при отправке некоторых файлов возникнут ошибки.

### <a name="example"></a>Пример

В этом примере приложение отправляет первые 26 из 128 байтов файла.

* Заголовок **Content-Length** задает размер текущего запроса.
* Заголовок **Content-Range** указывает диапазон (в байтах) для всего файла, представленного в запросе.
* Прежде чем отправлять первый фрагмент файла, необходимо знать общий размер этого файла.

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->

```http
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

**Важно!** Приложение должно указывать в заголовках **Content-Range** всех запросов один и тот же общий размер файла.
Если объявить для диапазона байтов другой размер файла, запрос не будет выполнен.

### <a name="response"></a>Ответ

После выполнения запроса сервер отправит в ответ код `202 Accepted`, если требуется отправить дополнительные диапазоны байтов.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

С помощью значения **nextExpectedRanges** приложение может определить, где должен начинаться следующий диапазон байтов.
Вы можете увидеть несколько диапазонов, указывающих части файла, еще не полученные сервером. Это удобно, когда требуется возобновить прерванную передачу, а клиенту неизвестно состояние службы.

Размер диапазонов байтов всегда следует определять в соответствии с приведенными ниже рекомендациями. Не рассчитывайте на то, что свойство **nextExpectedRanges** вернет диапазоны надлежащего размера для отправляемого диапазона байтов.
Свойство **nextExpectedRanges** указывает диапазоны файла, которые не были получены, а не схему отправки файла приложением.

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": [
  "12345-55232",
  "77829-99375"
  ]
}
```

## <a name="remarks"></a>Примечания

* В свойстве `nextExpectedRanges` не всегда указываются все отсутствующие диапазоны.
* При успешной записи фрагментов оно возвращает следующий диапазон (например, "523-").
* При сбоях в тех случаях, когда клиент отправляет файл, уже полученный сервером, сервер возвращает отклик `HTTP 416 Requested Range Not Satisfiable`. Вы можете [запросить состояние отправки](#resuming-an-in-progress-upload), чтобы получить более подробный список недостающих диапазонов.
* Как отклик на добавление заголовка авторизации при совершении вызова `PUT` может появиться сообщение об ошибке `HTTP 401 Unauthorized`. Заголовок авторизации и токен носителя необходимо отправлять только при выполнении `POST` на начальном этапе. Не следует включать их, когда совершается вызов `PUT`.

## <a name="completing-a-file"></a>Завершение отправки файла

После получения последнего диапазона байтов файла сервер отправляет отклик `HTTP 201 Created` или `HTTP 200 OK`.
Тело отклика также включает набор свойств по умолчанию для ресурса **driveItem**, представляющего полностью отправленный файл.

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-final", "scopes": "files.readwrite" } -->

```
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 21
Content-Range: bytes 101-127/128

<final bytes of the file>
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```

## <a name="handling-upload-conflicts"></a>Обработка конфликтов при отправке

В случае возникновения конфликта после отправки файла (например, если в ходе сеанса отправки был создан элемент с таким же именем) при отправке последнего диапазона байтов возвращается ошибка.

```http
HTTP/1.1 409 Conflict
Content-Type: application/json

{
  "error":
  {
    "code": "upload_name_conflict",
    "message": "Another file exists with the same name as the uploaded session. You can redirect the upload session to use a new filename by calling PUT with the new metadata and @microsoft.graph.sourceUrl attribute.",
  }
}
```

## <a name="cancel-the-upload-session"></a>Отмена сеанса отправки

Чтобы отменить сеанс отправки, отправьте запрос DELETE на URL-адрес отправки. При этом очищается временный файл, содержащий ранее отправленные данные. Это следует делать в тех случаях, когда отправка прерывается (например, если пользователь отменил передачу).

Временные файлы и соответствующий сеанс отправки автоматически очищаются по прошествии времени, указанного свойством **expirationDateTime**.
Временные файлы могут быть удалены не сразу по истечении срока действия.

### <a name="request"></a>Запрос

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->

```http
DELETE https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
```

### <a name="response"></a>Ответ

Ниже приводится пример отклика.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a>Возобновление выполняемой отправки

При отключении или сбое отправки до полного выполнения запроса все байты в этом запросе игнорируются. Это может произойти при разрыве соединения между приложением и службой. В этом случае приложение может возобновить передачу файла с ранее отправленного фрагмента.

Чтобы узнать, какие диапазоны байтов были получены ранее, приложение может запросить состояние сеанса отправки.

### <a name="example"></a>Пример

Получить состояние отправки можно, отправив запрос GET на адрес `uploadUrl`.

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```
GET https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF86633784148bb98a1zjcUhf7b0mpUadahs
```

В ответ сервер отправит список отсутствующих байтовых диапазонов, которые требуется отправить, и время окончания срока действия для сеанса отправки.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a>Отправка оставшихся данных

Теперь, когда приложению известно, с какого момента начинать отправку, возобновите операцию, выполнив действия из раздела [Отправка байтов в сеанс отправки](#upload-bytes-to-the-upload-session).

## <a name="handle-upload-errors"></a>Обработка ошибок отправки

После отправки последнего диапазона байтов файла может возникнуть ошибка. Она может быть вызвана конфликтом имен или превышением ограничения квоты.
Сеанс отправки будет сохранен до истечения срока его действия. Это позволяет приложению возобновить отправку, явно зафиксировав сеанс отправки.

Для этого приложение должно отправить запрос PUT с новым ресурсом **driveItem**, который будет использоваться при фиксации сеанса отправки.
Этот новый запрос должен устранить причину первоначальной ошибки отправки.

Чтобы указать, что приложение применяет существующий сеанс отправки, запрос PUT должен включать свойство `@microsoft.graph.sourceUrl` со значением URL-адреса сеанса отправки.

<!-- { "blockType": "ignored", "name": "explicit-upload-commit", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PUT /me/drive/root:/{path_to_parent}
Content-Type: application/json
If-Match: {etag or ctag}

{
  "name": "largefile.vhd",
  "@microsoft.graph.conflictBehavior": "rename",
  "@microsoft.graph.sourceUrl": "{upload session URL}"
}
```

**Примечание.** В этом вызове можно использовать заголовки `@microsoft.graph.conflictBehavior` и `if-match` надлежащим образом.

### <a name="http-response"></a>HTTP-отклик

Если файл можно зафиксировать с помощью новых метаданных, возвращается ответ `HTTP 201 Created` или `HTTP 200 OK` с метаданными ресурса Item для отправленного файла.

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```

## <a name="best-practices"></a>Рекомендации

* Возобновляйте или повторно запускайте операции отправки, не выполненные из-за разрывов соединения или каких-либо ошибок с кодом 5xx, в том числе:
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* Используйте стратегию экспоненциального откладывания, если при возобновлении или повторной отправке возвращаются ошибки сервера с кодом 5xx.
* При возникновении других ошибок не следует использовать эту стратегию. Вместо этого ограничьте количество повторных попыток.
* Для устранения ошибок `404 Not Found` при возобновляемой отправке начинайте всю отправку заново. Это означает, что сеанс отправки больше не существует.
* Используйте возобновляемую отправку для файлов размером более 10 МБ (10 485 760 байтов).
* Размер 10 МБ для диапазона байтов оптимален в случае стабильных высокоскоростных подключений. Если используется более медленное или менее надежное подключение, то вы можете получить оптимальные результаты, используя фрагменты меньшего размера. Рекомендуем использовать фрагменты размером 5–10 МБ.
* Используйте размер фрагментов, кратный 320 КБ (327 680 байтов). В противном случае после отправки последнего диапазона байтов большого файла может произойти сбой.

## <a name="error-responses"></a>Ответы с ошибками

Дополнительные сведения о том как возвращаются ошибки, см. в статье [Ошибки][error-response].

[error-response]: ../../../concepts/errors.md
[item-resource]: ../resources/driveitem.md
[fileSystemInfo]: ../resources/filesysteminfo.md;

<!-- {
  "type": "#page.annotation",
  "description": "Upload large files using an upload session.",
  "keywords": "upload,large file,fragment,BITS",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/driveitem_createuploadsession.md:
      Found potential enums in resource example that weren't defined in a table:(rename,fail,replace) are in resource, but () are in table"
  ],
  "section": "documentation"
} -->
