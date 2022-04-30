---
title: Вложение крупных файлов в сообщения и события Outlook
description: В зависимости от размера файла можно выбрать один из двух способов вложения файлов в сообщения или события.
author: abheek-das
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 582501205c106b3deaf0312f3db9c81488feb3de
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133050"
---
# <a name="attach-large-files-to-outlook-messages-or-events"></a>Вложение крупных файлов в сообщения и события Outlook

С помощью API Microsoft Graph можно вкладывать файлы размером до 150 МБ в элементы Outlook [сообщение](/graph/api/resources/message) или [событие](/graph/api/resources/event). В зависимости от размера файла выберите один из двух способов вложения файла:
- Если размер файла не превышает 3 МБ, выполните одну операцию POST в свойстве навигации **attachments** элемента Outlook. Узнайте, как это выполняется [для сообщения](/graph/api/message-post-attachments) или [события](/graph/api/event-post-attachments). Успешный отклик `POST` включает ИД вложенного файла.
- Если размер файла составляет от 3 до 150 МБ, создайте сеанс отправки и итеративно используйте `PUT` для отправки диапазонов байтов, пока не будет отправлен весь файл. Заголовок в итоговом успешном отклике `PUT` включает URL-адрес с ИД вложения.

Чтобы вложить в сообщение несколько файлов, выберите способ для каждого файла на основе их размеров и вложите файлы по отдельности.

В этой статье пошагово демонстрируется второй подход с созданием и использованием сеанса отправки для добавления большого вложенного файла (размером более 3 МБ) в элемент Outlook. На каждом шаге демонстрируется соответствующий код для сообщения и события. После успешной отправки целого файла в статье показано получение заголовка отклика, содержащего идентификатор вложения файла, который затем используется для получения необработанного содержимого или метаданных вложения. 

> [!IMPORTANT] 
> Обратите внимание на [известную проблему](known-issues.md#attaching-large-files-to-messages-with-delegated-permissions-can-fail) при вложении больших файлов в сообщение или событие в общем или делегированном почтовом ящике.

## <a name="step-1-create-an-upload-session"></a>Шаг 1. Создание сеанса отправки

[Создайте сеанс отправки](/graph/api/attachment-createuploadsession), чтобы вложить файл в сообщение или событие. Укажите файл во входном параметре **AttachmentItem**.

После успешной операции возвращается `HTTP 201 Created` и новый экземпляр объекта [uploadSession](/graph/api/resources/uploadsession), содержащий непрозрачный URL-адрес, который можно использовать в последующих операциях `PUT` для отправки частей этого файла. Этот экземпляр **uploadSession** предоставляет временное место хранения, где байты файла сохраняются до отправки всего файла.

Объект **uploadSession** в отклике также включает свойство **nextExpectedRanges**, указывающее, что начальное место отправки должно быть байтом 0.

### <a name="permissions"></a>Разрешения
Обязательно запросите разрешение `Mail.ReadWrite` на создание экземпляра **uploadSession** для сообщения и экземпляра `Calendars.ReadWrite` для события. 

Непрозрачный URL-адрес, возвращенный свойством **uploadUrl** нового объекта **uploadSession**, проходит предварительную проверку подлинности и содержит соответствующий маркер авторизации для последующих запросов `PUT` в домене `https://outlook.office.com`. Этот маркер истекает в срок **expirationDateTime**. Не следует изменять этот URL-адрес для операций `PUT`.


### <a name="example-create-an-upload-session-for-a-message"></a>Пример: создание сеанса отправки для сообщения

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "walkthrough_create_uploadsession_message",
  "sampleKeys": ["AAMkADI5MAAIT3drCAAA="]
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADI5MAAIT3drCAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower",
    "size": 3483322
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/walkthrough-create-uploadsession-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
В следующем примере отклика демонстрируется ресурс **uploadSession**, возвращаемый для сообщения.

<!-- {
  "blockType": "response",
  "name": "walkthrough_create_uploadsession_message",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
    "expirationDateTime": "2019-09-25T01:09:30.7671707Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```

### <a name="example-create-an-upload-session-for-an-event"></a>Пример: создание сеанса отправки для события
#### <a name="request"></a>Запрос 


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "walkthrough_create_uploadsession_event",
  "sampleKeys": ["AAMkADU5CCmSAAA="]
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkADU5CCmSAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower",
    "size": 3483322
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/walkthrough-create-uploadsession-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
В следующем примере отклика демонстрируется ресурс **uploadSession**, возвращаемый для события.

<!-- {
  "blockType": "response",
  "name": "walkthrough_create_uploadsession_event",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/v2.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/AttachmentSessions('AAMkADU5RpAACJlCs8AAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIBtw",
    "expirationDateTime": "2020-02-22T02:46:56.7410786Z",
    "nextExpectedRanges": [
        "0-"
    ]
}

```


## <a name="step-2-use-the-upload-session-to-upload-a-range-of-bytes-of-the-file"></a>Шаг 2. Отправка диапазона байтов файла с помощью сеанса отправки

Чтобы отправить файл или часть файла, выполните запрос `PUT` к URL-адресу, возвращенному на шаге 1 в свойстве **uploadUrl** ресурса **uploadSession**. Можно отправить файл целиком или разделить файл на несколько диапазонов байтов. Для более высокой производительности размер каждого диапазона байтов не должен превышать 4 МБ.

Укажите заголовки и основной текст запроса, как описано ниже.

### <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Content-Length | Int32 | Количество байтов, отправляемых в этой операции. Для более высокой производительности количество байт в каждой операции `PUT` не должно превышать 4 МБ. Обязательный элемент. |
| Content-Range | String | Диапазон байтов файла, отправляемого в этой операции, начиная с байта 0, выраженный в формате `bytes {start}-{end}/{total}`. Обязательно. |
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

### <a name="example-first-upload-to-the-message"></a>Пример: первая отправка в сообщение
#### <a name="request"></a>Запрос
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
Content-Type: application/octet-stream
Content-Length: 2097152
Content-Range: bytes 0-2097151/3483322

{
  <bytes 0-2097151 of the file to be attached, in binary format>
}
```

#### <a name="response"></a>Отклик

В следующем примере отклика в свойстве **NextExpectedRanges** демонстрируется начало следующего диапазона байтов, ожидаемого сервером.
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://outlook.office.com/api/v2.0/$metadata#Users('a8e8e219-4931-95c1-b73d-62626fd79c32%4072aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA%3D')/AttachmentSessions/$entity",
  "ExpirationDateTime":"2019-09-25T01:09:30.7671707Z",
  "NextExpectedRanges":["2097152"]
}
```

### <a name="example-first-upload-to-the-event"></a>Пример: первая отправка в событие
#### <a name="request"></a>Запрос
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/v2.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/AttachmentSessions('AAMkADU5RpAACJlCs8AAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIBtw
Content-Type: application/octet-stream
Content-Length: 2097152
Content-Range: bytes 0-2097151/3483322

{
  <bytes 0-2097151 of the file to be attached, in binary format>
}
```

#### <a name="response"></a>Отклик

В следующем примере отклика в свойстве **NextExpectedRanges** демонстрируется начало следующего диапазона байтов, ожидаемого сервером.
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://outlook.office.com/api/v2.0/$metadata#Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69%4098a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA%3D')/AttachmentSessions/$entity",
    "ExpirationDateTime":"2020-02-22T02:46:56.7410786Z",
    "NextExpectedRanges":["2097152"]
}
```


## <a name="step-3-continue-uploading-byte-ranges-until-the-entire-file-has-been-uploaded"></a>Шаг 3. Продолжение отправки диапазонов байтов вплоть до отправки всего файла

После первоначальной отправки на шаге 2 продолжайте отправлять оставшиеся части файла, используя аналогичный запрос `PUT`, как описано на шаге 2, до достижения даты и времени окончания срока действия сеанса. Получайте значение **NextExpectedRanges**, чтобы определить, с какого места должен начинаться следующий диапазон байтов для отправки. Вы можете увидеть несколько диапазонов, указывающих части файла, еще не полученные сервером. Это удобно, когда требуется возобновить прерванную передачу, а клиенту неизвестно состояние службы.

После успешной отправки последнего байта файла операция `PUT` возвращает `HTTP 201 Created` и заголовок `Location`, указывающий URL-адрес вложенного файла в домене `https://outlook.office.com`. Можно получить ИД вложения по этому URL-адресу и сохранить его для дальнейшего использования. В зависимости от сценария можно использовать этот ИД для [получения метаданных вложения](/graph/api/attachment-get) или для [удаления вложения из элемента Outlook](/graph/api/attachment-delete) с помощью конечной точки Microsoft Graph.

В следующих примерах показана отправка последнего диапазона байтов файла в сообщение и событие из предыдущих шагов.

### <a name="example-final-upload-to-the-message"></a>Пример: окончательная отправка в сообщение
#### <a name="request"></a>Запрос
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
Content-Type: application/octet-stream
Content-Length: 1386170
Content-Range: bytes 2097152-3483321/3483322

{
  <bytes 2097152-3483321 of the file to be attached, in binary format>
}
```

#### <a name="response"></a>Отклик
В следующем примере отклика показан заголовок отклика `Location`, из которого можно сохранить идентификатор вложения (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`) для дальнейшего применения.

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')
Content-Length: 0
```

### <a name="example-final-upload-to-the-event"></a>Пример: окончательная отправка в событие
#### <a name="request"></a>Запрос
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/v2.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/AttachmentSessions('AAMkADU5RpAACJlCs8AAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIBtw
Content-Type: application/octet-stream
Content-Length: 1386170
Content-Range: bytes 2097152-3483321/3483322

{
  <bytes 2097152-3483321 of the file to be attached, in binary format>
}
```

#### <a name="response"></a>Отклик
В следующем примере отклика показан заголовок отклика `Location`, из которого можно сохранить идентификатор вложения (`AAMkADU5CCmSAAANZAlYPeyQByv7Y=`) для дальнейшего применения.

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/v2.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/Attachments('AAMkADU5CCmSAAANZAlYPeyQByv7Y=')
Content-Length: 0
```

## <a name="step-4-optional-get-the-file-attachment-from-the-outlook-item"></a>Шаг 4 (необязательно). Получение вложенного файла из элемента Outlook

Как всегда, при [получении вложения](/graph/api/attachment-get) из элемента Outlook размер вложения не ограничивается технически.

Тем не менее, получение большого вложенного файла в формате кодировки base64 влияет на производительность API. Если ожидается вложение большого размера:

- Вместо получения вложенного содержимого в формате base64 можно [получить необработанные данные вложенного файла](/graph/api/attachment-get#example-6-get-the-raw-contents-of-a-file-attachment-on-a-message).
- Чтобы [получить метаданные вложенного файла](/graph/api/attachment-get#example-1-get-the-properties-of-a-file-attachment), добавьте параметр `$select`, включающий только нужные свойства метаданных, исключая свойство **contentBytes**, которое возвращает вложенный файл в формате base64.

### <a name="example-get-the-raw-file-attached-to-the-event"></a>Пример: получение необработанного файла, вложенного в событие
После примера события и использования идентификатора вложения, возвращаемого в заголовке `Location` предыдущего шага, в примере запроса в этом разделе демонстрируется использование параметра `$value` для получения необработанных данных содержимого вложения.

#### <a name="permissions"></a>Разрешения
Для этой операции необходимо использовать подходящее разрешение делегирования или приложения с минимальным уровнем привилегий, `Calendars.Read`. Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "ignored",
  "name": "walkthrough_get_attachment_raw",
  "sampleKeys": ["d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32", "AAMkADU5CCmSAAA=", "AAMkADU5CCmSAAANZAlYPeyQByv7Y="]
}-->
```http
GET https://graph.microsoft.com/v1.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/Attachments('AAMkADU5CCmSAAANZAlYPeyQByv7Y=')/$value
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "ignored",
  "name": "walkthrough_get_attachment_raw",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
content-length: 3483322
Content-type: image/jpeg

{Raw bytes of the file}
```


### <a name="example-get-the-metadata-of-the-file-attached-to-the-message"></a>Пример: получение метаданных файла, вложенного в сообщение
После примера сообщения в примере запроса в этом разделе демонстрируется использование параметра `$select` для получения некоторых метаданных файла, вложенного в сообщение, кроме **contentBytes**.

#### <a name="permissions"></a>Разрешения
Для этой операции необходимо использовать подходящее разрешение делегирования или приложения с минимальным уровнем привилегий, `Mail.Read` Дополнительные сведения см. в разделе [Разрешения почты](permissions-reference.md#mail-permissions).

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "walkthrough_get_attachment_metadata",
  "sampleKeys": ["a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47", "AAMkADI5MAAIT3drCAAA=", "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0="]
}-->
```http
GET https://graph.microsoft.com/api/v1.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')?$select=lastModifiedDateTime,name,contentType,size,isInline
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "name": "walkthrough_get_attachment_metadata",
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
    "isInline": false
}
```


## <a name="alternative-cancel-the-upload-session"></a>Альтернатива: отмена сеанса отправки

Если необходимо отменить отправку в любое время до окончания срока действия сеанса отправки, можно использовать тот же самый начальный непрозрачный URL-адрес, чтобы удалить сеанс отправки. После успешной операции возвращается `HTTP 204 No Content`.

### <a name="permissions"></a>Разрешения
Поскольку исходный непрозрачный URL-адрес прошел предварительную проверку подлинности и содержит подходящий маркер авторизации для последующих запросов для этого сеанса отправки, не указывайте заголовок запроса на авторизацию для этой операции.

### <a name="example-cancel-the-upload-session-for-the-message"></a>Пример: отмена сеанса отправки для сообщения

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "ignored"
}-->
```http
DELETE https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 204 No content
```
## <a name="errors"></a>Ошибки

### <a name="errorattachmentsizeshouldnotbelessthanminimumsize"></a>ErrorAttachmentSizeShouldNotBeLessThanMinimumSize

Эта ошибка возвращается при попытке [создать сеанс отправки](/graph/api/attachment-createuploadsession), чтобы вложить файл размером менее 3 МБ. Если размер файла меньше 3 МБ, следует выполнить одну операцию POST для свойства навигации **attachments** [сообщения](/graph/api/message-post-attachments) или [события](/graph/api/event-post-attachments). Успешный отклик `POST` включает ИД файла, прикрепленного к сообщению.

