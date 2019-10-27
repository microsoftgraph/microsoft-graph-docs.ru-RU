---
title: Вложение крупных файлов в сообщения Outlook
description: В зависимости от размера файла можно выбрать один из двух способов вложения файла в сообщение.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 62d5496ba3e7a1ccb28af45922a254a6d10c6519
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2019
ms.locfileid: "37726517"
---
# <a name="attach-large-files-to-outlook-messages-as-attachments-preview"></a>Прикрепление крупных файлов к сообщениям Outlook в виде вложений (предварительная версия)

В зависимости от размера файла можно выбрать один из двух способов вложения файлов в [сообщения](/graph/api/resources/message?view=graph-rest-beta).

- Если размер файла меньше 4 МЬ, можно выполнить одну операцию [POST для свойства навигации вложений сообщения](/graph/api/message-post-attachments?view=graph-rest-beta). Успешный отклик `POST` включает ИД файла, прикрепленного к сообщению.
- Если размер файла составляет от 3 до 150 МБ, создайте сеанс отправки и итеративно используйте `PUT` для отправки диапазонов байтов, пока не будет отправлен весь файл. Заголовок в итоговом успешном отклике `PUT` включает URL-адрес с ИД вложения. 

В этой статье используется пример для иллюстрации второго подхода. В этом примере создается и используется сеанс отправки, чтобы добавить большой файл (размером свыше 3 МБ) к определенному сообщению в качестве вложения. После успешной отправки всего файла возвращается URL-адрес с ИД вложения, с которыми можно выполнять другие операции, например получать метаданные о вложенном файле.

## <a name="step-1-create-an-upload-session"></a>Шаг 1. Создайте сеанс отправки.

[Создайте сеанс отправки](/graph/api/attachment-createuploadsession?view=graph-rest-beta), чтобы вложить файл в сообщение. Укажите файл во входном параметре **AttachmentItem**. 

После успешной операции возвращается `HTTP 201 Created` и новый экземпляр объекта [uploadSession](/graph/api/resources/uploadsession?view=graph-rest-beta), содержащий непрозрачный URL-адрес, который можно использовать в последующих операциях `PUT` для отправки частей этого файла. Этот экземпляр **uploadSession** предоставляет временное место хранения, где байты файла сохраняются до отправки всего файла. 

Непрозрачный URL-адрес, возвращенный свойством **uploadUrl** объекта **uploadSession**, проходит предварительную проверку подлинности и содержит соответствующий маркер авторизации для последующих запросов `PUT` в домене `https://outlook.office.com`. Этот маркер истекает в срок **expirationDateTime**. Не следует изменять этот URL-адрес для операций `PUT`.

Объект **uploadSession** в отклике также включает свойство **nextExpectedRanges**, указывающее, что начальное место отправки должно быть байтом 0.

### <a name="example-request-create-an-upload-session"></a>Пример запроса: создание сеанса отправки

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "walkthrough_create_uploadsession",
  "sampleKeys": ["AAMkADI5MAAIT3drCAAA="]
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAIT3drCAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower", 
    "size": 3483322
  }
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="example-response-get-an-uploadsession-object"></a>Пример отклика: получение объекта uploadSession
<!-- {
  "blockType": "response",
  "name": "walkthrough_create_uploadsession",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
    "expirationDateTime": "2019-09-25T01:09:30.7671707Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```


## <a name="step-2-use-the-upload-session-to-upload-a-range-of-bytes-of-the-file"></a>Шаг 2. Используйте сеанс отправки, чтобы отправить диапазон байтов файла.

Чтобы отправить файл или часть файла, сделайте запрос `PUT` к значению свойства **uploadUrl**, возвращенному в составе **uploadSession** на шаге 1. Можно отправить файл целиком или разделить файл на несколько диапазонов байтов. Для более высокой производительности размер каждого диапазона байтов не должен превышать 4 МБ. 

Укажите заголовки и основной текст запроса, как описано ниже.

### <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Content-Length | Int32 | Количество байтов, отправляемых в этой операции. Для более высокой производительности количество байт в каждой операции `PUT` не должно превышать 4 МБ. Обязательный элемент. |
| Content-Range | String | Диапазон байтов файла, отправляемого в этой операции, начиная с байта 0, выраженный в формате `bytes {start}-{end}/{total}`. Обязательный элемент. |
| Content-Type | String  | Тип MIME. Укажите `application/octet-stream`. Обязательный элемент. |

Не указывайте заголовок запроса `Authorization`. Запрос `PUT` использует прошедший предварительную проверку подлинности URL-адрес из свойства **uploadUrl**, что позволяет получить доступ к домену `https://outlook.office.com`.

### <a name="request-body"></a>Основной текст запроса

Укажите фактические байты вкладываемого файла, находящиеся в диапазоне расположения, указанном в заголовке запроса `Content-Range`.

### <a name="response"></a>Отклик
После успешной отправки возвращается `HTTP 200 OK` и объект **uploadSession**. Объект отклика имеет указанные ниже свойства.

- Свойство **ExpirationDateTime** указывает дату и время окончания срока действия для маркера авторизации, внедренного в значение свойства **uploadUrl**. Это значение даты и времени окончания срока действия остается таким же, какое было возвращено начальным объектом **uploadSession** на шаге 1. 
- Свойство **NextExpectedRanges** указывает расположение следующего байта, с которого необходимо начать отправку, например `"NextExpectedRanges":["2097152"]`. Байты файла необходимо отправлять по порядку.
<!-- The **NextExpectedRanges** specifies one or more byte ranges, each indicating the starting point of a subsequent `PUT` request:

  - On a successful upload, this property returns the next range to start from, for example, `"NextExpectedRanges":["2097152"]`. 
  - If a portion of a byte range has not uploaded successfully, this property includes the byte range with the start and end locations, for example, `"NextExpectedRanges":["1998457-2097094"]`.
-->
- Свойство **uploadUrl** не возвращается явным образом, поскольку все операции `PUT` сеанса отправки используют тот же самый URL-адрес, который был возвращен при создании сеанса (на шаге 1).

### <a name="example-request-first-upload"></a>Пример запроса: первая отправка
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
Content-Type: application/octet-stream
Content-Length: 2097152
Content-Range: bytes 0-2097151/3483322

{
  <bytes 0-2097151 of the file to be attached, in binary format>
}
```

### <a name="example-response-get-the-start-of-the-next-byte-range-that-the-server-expects"></a>Пример отклика: получение начала следующего диапазона байтов, ожидаемого сервером
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://outlook.office.com/api/beta/$metadata#Users('a8e8e219-4931-95c1-b73d-62626fd79c32%4072aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA%3D')/AttachmentSessions/$entity",
  "ExpirationDateTime":"2019-09-25T01:09:30.7671707Z",
  "NextExpectedRanges":["2097152"]
}
```


## <a name="step-3-continue-uploading-byte-ranges-until-the-entire-file-has-been-uploaded"></a>Шаг 3. Продолжение отправки диапазонов байтов вплоть до отправки всего файла.

После первоначальной отправки на шаге 2 продолжайте отправлять оставшиеся части файла, используя аналогичный запрос `PUT`, как описано на шаге 2, до достижения даты и времени окончания срока действия сеанса. Получайте значение **NextExpectedRanges**, чтобы определить, с какого места должен начинаться следующий диапазон байтов для отправки. Вы можете увидеть несколько диапазонов, указывающих части файла, еще не полученные сервером. Это удобно, когда требуется возобновить прерванную передачу, а клиенту неизвестно состояние службы.

После успешной отправки последнего байта файла операция `PUT` возвращает `HTTP 201 Created` и заголовок `Location`, указывающий URL-адрес вложенного файла в домене `https://outlook.office.com`. Можно получить ИД вложения по этому URL-адресу и сохранить его для дальнейшего использования. В зависимости от сценария можно использовать этот ИД для [получения метаданных вложения](/graph/api/attachment-get?view=graph-rest-beta) или для [удаления уложения из сообщения](/graph/api/attachment-delete?view=graph-rest-beta) с помощью конечной точки Microsoft Graph.

В следующем примере показана отправка последнего байтового диапазона файла.

### <a name="example-request-final-upload"></a>Пример запроса: окончательная отправка
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
Content-Type: application/octet-stream
Content-Length: 1386170
Content-Range: bytes 2097152-3483321/3483322

{
  <bytes 2097152-3483321 of the file to be attached, in binary format>
}
```

### <a name="example-response-get-the-location-response-header-to-save-the-attachment-id"></a>Пример отклика: получения заголовка отклика Location для сохранения ИД вложения.

URL-адрес, указанный заголовком отклика `Location`, содержит ИД вложения (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`). Сохраните его для дальнейшего использования.

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')
Content-Length: 0
```

## <a name="step-4-optional-get-the-file-attachment-from-the-message"></a>Шаг 4 (необязательно). Получение вложенного файла из сообщения.

Как всегда, при [получении вложения](/graph/api/attachment-get?view=graph-rest-beta) из сообщения размер вложения не ограничивается технически. 

Тем не менее, получение большого вложенного файла в формате кодировки base64 влияет на производительность API. Если ожидается вложение большого размера:
 
- Вместо получения вложенного содержимого в формате base64 можно [получить необработанные данные вложенного файла](/graph/api/attachment-get#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message?view=graph-rest-1.0).
- Чтобы [получить метаданные вложенного файла](/graph/api/attachment-get?view=graph-rest-beta#example-1-get-the-properties-of-a-file-attachment), добавьте параметр `$select`, включающий только нужные свойства метаданных, исключая свойство **contentBytes**, которое возвращает вложенный файл в формате base64.

### <a name="example-request-get-the-file-attachment-metadata"></a>Пример запроса: получение метаданных вложенного файла

В следующем примере отправитель использует параметр `$select` для получения всех метаданных файла, вложенного в сообщение, кроме свойства **contentBytes**.

<!-- {
  "blockType": "request",
  "name": "walkthrough_get_attachment", 
  "sampleKeys": ["a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47", "AAMkADI5MAAIT3drCAAA=", "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0="]
}-->
```http
GET https://graph.microsoft.com/api/v1.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')?$select=lastModifiedDateTime,name,contentType,size,isInline,contentId,contentLocation
```

### <a name="example-response"></a>Пример отклика

<!-- {
  "blockType": "response",
  "name": "walkthrough_get_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('a8e8e219-4931-95c1-b73d-62626fd79c32%4072aa88bf-76f0-494f-91ab-2d7cd730db47')/messages('AAMkADI5MAAIT3drCAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.fileAttachment",
    "@odata.mediaContentType": "image/jpeg",
    "id": "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=",
    "lastModifiedDateTime": "2019-09-24T23:27:43Z",
    "name": "flower",
    "contentType": "image/jpeg",
    "size": 3640066,
    "isInline": false,
    "contentId": null,
    "contentLocation": null
}
```

## <a name="alternative-cancel-the-upload-session"></a>Альтернатива: отмена сеанса отправки

Если необходимо отменить отправку в любое время до окончания срока действия сеанса отправки, можно использовать тот же самый начальный непрозрачный URL-адрес, чтобы удалить сеанс отправки. После успешной операции возвращается `HTTP 204 No Content`.

### <a name="example-request-cancel-an-upload-session"></a>Пример запроса: отмена сеанса отправки

<!-- {
  "blockType": "ignored"
}-->
```http
DELETE https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
```

### <a name="example-response"></a>Пример отклика

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 204 No content
```


