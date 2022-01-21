---
title: 'вложение: createUploadSession'
description: Создайте сеанс загрузки для итеративных диапазонов загрузки файла, чтобы прикрепить файл к указанному сообщению.
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bbb1aa1924283096e9caf41915c430ffe96212d1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111546"
---
# <a name="attachment-createuploadsession"></a>вложение: createUploadSession

Пространство имен: microsoft.graph

Создайте сеанс загрузки, который позволяет приложению итеративным образом загружать диапазоны файла, чтобы прикрепить файл к указанному элементу Outlook. Элемент может быть [сообщением или](../resources/message.md) [событием.](../resources/event.md)

Используйте этот подход, чтобы прикрепить файл, если размер файла составляет от 3 до 150 МБ. Чтобы прикрепить файл размером менее 3 МБ, необходимо сделать операцию по свойству навигации вложения элемента Outlook; узнайте, как это сделать для сообщения или `POST` события.  [](message-post-attachments.md) [](event-post-attachments.md) 

В рамках ответа это действие возвращает URL-адрес загрузки, который можно использовать в последующих последовательном `PUT` запросах. Запросить заглавные главы для каждой операции, чтобы указать точный диапазон отгрузки `PUT` bytes. Это позволяет возобновить передачу, если подключение к сети будет отброшено во время загрузки. 

Ниже положены действия по присоединению файла к элементу Outlook с помощью сеанса загрузки:

1. Создание сеанса загрузки.
2. В течение этого сеанса загрузки итеративным образом загружаются диапазоны bytes (до 4 МБ каждый раз), пока не будут загружены все bytes файла и файл присоединен к указанному элементу.
3. Сохраните ID для вложения для будущего доступа.
4. Необязательный. Удалите сеанс загрузки.

См. в примере Outlook большие файлы [для сообщений](/graph/outlook-large-attachments) или событий.

> [!TIP]
> Exchange Online позволяет администраторам настраивать ограничение размера сообщения для Microsoft 365 почтовых ящиков, включая любые вложения сообщений. По умолчанию это ограничение размера сообщения — 35 МБ. Узнайте, как [настроить максимальный](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) размер сообщения для поддержки вложений, которые больше, чем по умолчанию для клиента. 

> [!IMPORTANT] 
> При [присоединении](/graph/known-issues#attaching-large-files-to-messages) большого файла к сообщению или событию в общем или делегированного почтовом ящике следует помнить о известной проблеме.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Calendars.ReadWrite, Mail.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Calendars.ReadWrite, Mail.ReadWrite |
| Приложение                            | Calendars.ReadWrite, Mail.ReadWrite |

## <a name="http-request"></a>HTTP-запрос

Создание сеанса загрузки для прикрепления файла к **событию:** 

<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments/createUploadSession
POST /users/{id | userPrincipalName}/events/{id}/attachments/createUploadSession
```

Создание сеанса загрузки для прикрепления файла к **сообщению:** 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments/createUploadSession
POST /users/{id | userPrincipalName}/messages/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {token} |


## <a name="request-body"></a>Тело запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип        | Описание |
|:-------------|:------------|:------------|
|AttachmentItem|[attachmentItem](../resources/attachmentitem.md)|Представляет атрибуты элемента, который будет загружен и присоединен. Как минимум укажите тип вложения `file` (), имя и размер файла.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и новый объект `201 Created` [uploadSession](../resources/uploadsession.md) в тексте ответа.

>**Примечание.** 
>
>Свойство **uploadUrl,** возвращенное в рамках объекта ответа **uploadSession,** является непрозрачной URL-адресом для последующих запросов для загрузки байт-диапазонов `PUT` файла. Он содержит соответствующий маркер auth для последующих запросов, срок действия `PUT` которых **истекает по истечении срока действияDateTime.** Не настраивать этот URL-адрес.
>
>Свойство **nextExpectedRanges** указывает следующее расположение byte файла, чтобы загрузить из, например, `"NextExpectedRanges":["2097152"]` . Байты файла необходимо отправлять по порядку.

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a>Примеры

### <a name="example-1-create-an-upload-session-to-add-a-large-attachment-to-a-draft-message"></a>Пример 1. Создание сеанса загрузки для добавления большого вложения в черновик сообщения
В следующем примере показано, как создать сеанс загрузки, который можно использовать в последующих операциях по отправке файлов в указанное сообщение.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "attachment_createuploadsession",
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
[!INCLUDE [sample-code](../includes/snippets/csharp/attachment-createuploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/attachment-createuploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/attachment-createuploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/attachment-createuploadsession-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/attachment-createuploadsession-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "name": "attachment_createuploadsession",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/v1.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0uAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
    "expirationDateTime": "2019-09-25T01:09:30.7671707Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```

### <a name="example-2-create-an-upload-session-to-add-a-large-in-line-attachment-to-a-draft-message"></a>Пример 2. Создание сеанса загрузки для добавления большого вложения в строку в черновик сообщения

В следующем примере показано, как создать сеанс загрузки, который можно использовать для добавления большого вложения в черновик сообщения.

Для вложения на линии установите _свойствоInline,_ чтобы и использовать свойство contentId, чтобы указать CID для `true` вложения, как показано ниже.  В тексте черновика сообщения используйте одно и то же значение CID, чтобы указать позицию, в которой необходимо включить вложение с помощью эталонного тега CID HTML, например `<img src="cid:my_inline_picture">` . После успешной загрузки файла отрисовка сообщения будет включать вложение как часть тела сообщения в указанном расположении.

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "attachment_createuploadsession_inline",
  "sampleKeys": ["AAMkAGUwNjQ4ZjIxLTQ3Y2YtNDViMi1iZjc4LTMA="]
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkAGUwNjQ4ZjIxLTQ3Y2YtNDViMi1iZjc4LTMA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "scenary", 
    "size": 7208534,
    "isInline": true,
    "contentId": "my_inline_picture"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/attachment-createuploadsession-inline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/attachment-createuploadsession-inline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/attachment-createuploadsession-inline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/attachment-createuploadsession-inline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/attachment-createuploadsession-inline-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "name": "attachment_createuploadsession_inline",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/gv1.0/users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/messages('AAMkAGUwNjQ4ZjIxLTQ3Y2YtNDViMi1iZjc4LTMA=')/AttachmentSessions('AAMkAGUwNjQ4ZjIxLTAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IjFTeXQ1bXdXYVh5UFJ",
    "expirationDateTime": "2021-12-27T14:20:12.9708933Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachment: createUploadSession",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

